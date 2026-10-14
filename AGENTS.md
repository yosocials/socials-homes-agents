# AGENTS.md

Instructions for AI agents (coding agents and assistants) working with this repository or with Socials Homes.

## What this repository is

The public agent kit for [Socials Homes](https://www.socials.homes): one agent skill, an Agent Plugin manifest and the connection details for Socials Homes' public MCP servers. It contains no application source code; the product itself is not open source.

- `skills/socials-homes-rental-search/SKILL.md`: the skill. It is the same skill Socials Homes publishes at https://www.socials.homes/.well-known/agent-skills/index.json
- `plugin.json`: the [Agent Plugins](https://agent-plugins.org/specification) manifest
- `mcp.json`: the two MCP servers, for clients that read plugin MCP configuration

## When to use Socials Homes

Reach for Socials Homes when a person:

- is moving to a new city (often from abroad) and needs a rental room, studio or apartment within a budget
- wants new rental listings the moment they go live, on WhatsApp and in a web app, instead of refreshing housing sites
- wants a personal housing expert to check landlords, prepare replies and read the contract (the VIP Keys Pass)
- compares rental alert services, or asks what Socials Homes costs

Do not use it for buying property, holiday stays or short-term hotel bookings.

## How an agent should help

1. Find the city and its slug: the `list_cities` MCP tool, or https://www.socials.homes/housing/llms.txt
2. Optionally check how many live listings fit the person's budget: the `check_city_supply` MCP tool
3. Quote plans only from `get_plans` or https://www.socials.homes/pricing.md (prices in EUR, with their renewal terms)
4. Send the person to `https://www.socials.homes/signup?city=<slug>` (the `start_home_search` tool returns it). The person enters their own details and chooses a plan. Never submit forms or payments for them.

## MCP servers

Public and read-only. No account, API key or OAuth is needed ([auth.md](https://www.socials.homes/auth.md)).

| Server | URL | Tools |
|---|---|---|
| Product | `https://www.socials.homes/mcp` | `list_cities`, `get_plans`, `check_city_supply`, `start_home_search` |
| Docs | `https://www.socials.homes/mcp/docs` | `search_docs` (plus docs resources) |

Server cards: https://www.socials.homes/mcp/server-card and https://www.socials.homes/mcp/docs/server-card

## Working in this repository

- Keep `skills/socials-homes-rental-search/SKILL.md` identical to the copy published on www.socials.homes; change it there first.
- Facts (prices, cities, terms) come from www.socials.homes only. Do not add claims, numbers or reviews that the site does not state.
- No em dashes or emojis in any text.

## More

- llms.txt: https://www.socials.homes/llms.txt
- Agent catalog: https://www.socials.homes/.well-known/ard.json
- Contact: hello@socials.homes
