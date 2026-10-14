---
name: socials-homes-city-supply
description: "Check whether Socials Homes covers a city and how many live rental listings there are in it, optionally at or under a monthly budget in EUR, using the public read-only Socials Homes MCP server. Use when a person moving to a new city asks if there are rooms, studios or apartments within their budget, which cities are covered, or whether their budget is realistic before they start a rental search."
license: Proprietary
metadata:
  publisher: "Socials Homes"
  homepage: "https://www.socials.homes"
  contact: "hello@socials.homes"
---

# Check rental supply in a city with Socials Homes

Socials Homes scans 2,000+ housing sites in 124 cities and keeps a live count of the listings it can see. This skill answers "is there anything in my city within my budget?" before a person starts a search.

## Tools

The Socials Homes MCP server is public and read-only, with no sign-in: `https://www.socials.homes/mcp` (Streamable HTTP).

1. `list_cities` returns every covered city with its slug, name and country. Filter with `country` (an ISO code such as `NL` or a name such as `Netherlands`).
2. `check_city_supply` takes `city` (a slug, or a city name, including local names such as `Den Haag`) and optional `budget_max_eur`, and returns the live listing count for the city and the count at or under the budget.
3. `start_home_search` returns the signup link for a city. It creates and sends nothing.

Without MCP, the city list is at https://www.socials.homes/housing/llms.txt and each city has a markdown page at `https://www.socials.homes/housing/<city>.md`.

## How to answer

1. Confirm the city and the person's monthly budget in EUR.
2. Call `check_city_supply`. Report both numbers plainly, for example: "Berlin has about 7,000 live listings; about 4,400 are at or under €800 a month."
3. If the count under budget is low, say so and mention the suggested budget the tool returns, if any. Never promise that a home will be found.
4. If the tool says data is unavailable, say the count is unavailable right now. Never treat that as zero.
5. Counts cover the housing sites Socials Homes scans, not every listing in the city. Say this when it matters.
6. To start a search, give the signup link from `start_home_search`. The person enters their own details and chooses a plan.

## Limits

The MCP server allows 300 requests a minute per IP, and `check_city_supply` 600 an hour per IP. Over the limit it answers HTTP 429 with Retry-After. Access details: https://www.socials.homes/auth.md
