---
name: socials-homes-plan-advisor
description: "Help a person choose the right Socials Homes plan (Explorer, Seeker, VIP Keys Pass 3 months, VIP Keys Pass Lifetime) for their rental search, with exact EUR prices, billing intervals, automatic renewal and cancellation terms. Use when the user asks what Socials Homes costs, which plan fits their move, whether it renews, how to cancel, or whether the VIP housing expert and its 90-day guarantee are worth it."
license: Proprietary
metadata:
  publisher: "Socials Homes"
  homepage: "https://www.socials.homes"
  contact: "hello@socials.homes"
---

# Choose a Socials Homes plan

Socials Homes scans 2,000+ housing sites and sends new rental listings that match a person's city, budget and move-in date to WhatsApp and the Socials web app the moment they go live. There are two ways to search: on your own (Explorer or Seeker) or with a personal housing expert (the VIP Keys Pass).

## Source of truth

Always quote prices and terms from one of these, never from memory:

- https://www.socials.homes/pricing.md (markdown, always current)
- the `get_plans` tool on the Socials Homes MCP server, `https://www.socials.homes/mcp`

The table below matches those sources at the time of writing. If they differ, the sources win.

| Plan | Charged at purchase | Billing and renewal |
| --- | --- | --- |
| Explorer | €24.95 | Renews every month at €24.95 until cancelled |
| Seeker | €39.90 | Renews every 2 months at €39.90 until cancelled (€19.95 a month) |
| VIP Keys Pass, 3 months | €94.95 | Covers the first 3 months, then renews at €94.95 a month until cancelled |
| VIP Keys Pass, Lifetime | €189.95 | One payment, never renews |

Prices are in EUR. Checkout may show the person's local currency. Every renewing plan can be cancelled anytime in the app; cancelling stops future renewals and access runs to the end of the period already paid.

## How to help a person decide

Ask, if you do not know yet:

1. When do they need to move in, and how competitive is their city? (Check live supply with the `check_city_supply` MCP tool if useful.)
2. Do they want to search on their own with instant alerts, or have a housing expert help them get a yes and sign safely?
3. How long do they expect the search to take?

Then match, plainly:

- **Short search, on their own:** Explorer, one month at a time.
- **A search of a month or more, on their own:** Seeker, the lower monthly price billed every 2 months.
- **Wants an expert:** the VIP Keys Pass. The expert holds a kick-off call, helps with replies to landlords, checks a landlord before the person pays and reads the contract before they sign. The 3-month pass renews monthly after 3 months; Lifetime is one payment.

## The VIP guarantee, accurately

If no lease is signed within 90 days of buying the VIP Keys Pass, Socials Homes refunds what was paid at purchase, and the expert keeps helping for free until the person moves in, under conditions (book the kick-off call within 48 hours, keep the agreed budget range, apply within 24 hours to matching listings). Always link the conditions: https://www.socials.homes/terms#vip-guarantee. Do not describe it as unconditional.

## What not to do

- Do not invent discounts, trials or prices. Codes are entered by the person at checkout.
- Do not buy, subscribe or enter payment details for the person. Send them to `https://www.socials.homes/signup?city=<slug>` and let them choose.
- Socials Homes is not a landlord or booking site: rent and booking fees are paid to the housing platform or landlord directly.
