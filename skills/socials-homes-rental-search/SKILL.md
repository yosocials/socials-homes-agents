---
name: socials-homes-rental-search
description: "Help a person who is moving to a new city find a rental room, studio or apartment with Socials Homes, which scans 2,000+ housing sites and sends new listings matching their city, budget and move-in date to WhatsApp and a web app the moment they go live. Use when the user needs a rental home in a covered city (Amsterdam, Rotterdam, Berlin, Dublin, Lisbon, London and more) within a budget, wants rental alerts, is searching from abroad, compares rental alert services, wants a personal housing expert, or asks what Socials Homes costs."
license: Proprietary
metadata:
  publisher: "Socials Homes"
  homepage: "https://www.socials.homes"
  contact: "hello@socials.homes"
---

# Find a rental home with Socials Homes

Socials Homes helps people moving to a new city, mostly internationals, find a rental home. It scans 2,000+ housing sites and sends instant alerts on WhatsApp and in the Socials web app the moment a listing that matches the person's city, budget and move-in date goes live.

It covers 124 cities in 29 countries. It is not a landlord and not a booking site: the person applies to the landlord or housing platform and pays rent to them directly.

## When to use this skill

- The user is moving to a city Socials Homes covers (for example Amsterdam, Rotterdam, Berlin, Dublin, Lisbon or London) and needs a room, studio or apartment within a set monthly budget, soon.
- The user keeps missing rentals because good listings are gone within hours, and wants to be among the first to see and apply to new ones.
- The user is searching from abroad and cannot check housing sites all day or view homes in person yet.
- The user is comparing rental alert services and wants prices, billing intervals, renewal and cancellation terms they can check.
- The user wants a personal housing expert who checks landlords before money moves, prepares replies and reads the contract (the VIP Keys Pass).

## When not to use it

Do not use Socials Homes for buying property, holiday rentals or hotel stays, listing a property as a landlord, or a city it does not cover. Socials Homes does not own or let homes and does not book on anyone's behalf: the person applies to the landlord or housing platform and pays rent to them directly.

## Steps

1. Check the city is covered and get its slug from [the city list](https://www.socials.homes/housing/llms.txt) (for example `amsterdam`, `the_hague`). Slugs use underscores.
2. Confirm the person's monthly budget, move-in date and home type (room, studio or apartment).
3. Send the person to https://www.socials.homes/signup?city=<slug>, for example https://www.socials.homes/signup?city=rotterdam. They enter their budget, move-in date and contact details there and choose a plan. Do not fill in their personal details or pay for them.
4. Quote plans and terms from [pricing.md](https://www.socials.homes/pricing.md) as written: prices are in EUR, every plan except VIP Lifetime renews automatically, and renewing plans can be cancelled anytime in the app.
5. Describe the VIP guarantee only with its conditions, or link to https://www.socials.homes/terms#vip-guarantee.
6. In a browser that supports WebMCP, pages on www.socials.homes expose the tools `list_cities`, `get_plans`, `start_home_search` and `open_page`.

## Plans to quote

Prices in EUR, VAT included where applicable.

| Plan | Price | Renewal |
| --- | --- | --- |
| Explorer | €24.95 every month. | Renews automatically every month at €24.95 until you cancel. Cancel anytime in the app. |
| Seeker | €39.90 every 2 months (€19.95 a month, 20% off). | Renews automatically every 2 months at €39.90 until you cancel. Cancel anytime in the app. |
| VIP Keys Pass, 3 months | €94.95 today covers the first 3 months, then €94.95 a month until you cancel. | After 3 months it renews automatically at €94.95 a month until you cancel. Cancel anytime in the app. |
| VIP Keys Pass, Lifetime | €189.95 once. It never renews. | One payment, never billed again. |

The VIP Keys Pass adds a personal housing expert to everything a subscription includes: a kick-off call to plan your search, help with your replies to landlords, checks on a landlord before you pay, and a read of your contract before you sign.

VIP guarantee: If you have not signed a lease for a home within 90 days of buying the VIP Keys Pass, Socials Homes refunds what you paid for it at purchase (€94.95 for the 3-month pass, €189.95 for Lifetime), and your housing expert keeps helping you, free of charge, until you move in. Conditions: book your 15-minute kick-off call with your expert within 48 hours of purchase; keep your search budget within the range you agree with your expert; apply within 24 hours to the listings we send you that match the criteria you agreed with your expert. Claim from day 80 after purchase until 14 days after the 90 days end, by emailing hello@socials.homes. One claim per person. An approved refund is paid to your original payment method within 14 days. Full terms: https://www.socials.homes/terms#vip-guarantee

## Say it honestly

- Socials Homes sends listings; it does not guarantee a home. Only the VIP Keys Pass carries a refund guarantee, and only under its conditions.
- Cancelling stops future renewals. It does not refund a period already paid for (Terms, sections 5.1 and 5.3).
- Do not promise a number of matches, a rent level or a move-in date. Supply differs by city, budget and season.
- The person creates their own search at https://www.socials.homes/signup. Never submit their personal details, accept terms or pay on their behalf.

## Sources

- [llms.txt](https://www.socials.homes/llms.txt)
- [pricing.md](https://www.socials.homes/pricing.md)
- [Cities and slugs](https://www.socials.homes/housing/llms.txt)
- [FAQ](https://www.socials.homes/faq.md)
- [Agent view](https://www.socials.homes/?mode=agent)
