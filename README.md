# Socials Homes agent kit

Everything an AI agent needs to help a person find a rental home with [Socials Homes](https://www.socials.homes): Socials Homes scans 2,000+ housing sites and sends new listings matching a person's city, budget and move-in date to WhatsApp and a web app the moment they go live.

This repository holds no application code. It contains:

- **An agent skill**: [`skills/socials-homes-rental-search/SKILL.md`](skills/socials-homes-rental-search/SKILL.md)
- **An Agent Plugin manifest**: [`plugin.json`](plugin.json) and [`mcp.json`](mcp.json)
- **Agent instructions**: [`AGENTS.md`](AGENTS.md)

## Install the skill

```bash
npx skills add yosocials/socials-homes-agents
```

## Connect the MCP servers

Public, read-only, no sign-in:

- Product: `https://www.socials.homes/mcp` (`list_cities`, `get_plans`, `check_city_supply`, `start_home_search`)
- Docs: `https://www.socials.homes/mcp/docs` (`search_docs`)

Add either as a remote MCP server (Streamable HTTP) in Claude, ChatGPT or any MCP client.

## Links

- Website: https://www.socials.homes
- llms.txt: https://www.socials.homes/llms.txt
- Pricing (markdown): https://www.socials.homes/pricing.md
- Access and limits: https://www.socials.homes/auth.md
- Contact: hello@socials.homes

[![skills.sh](https://skills.sh/b/yosocials/socials-homes-agents)](https://skills.sh/yosocials/socials-homes-agents)
