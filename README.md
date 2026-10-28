# Ohmbo plugin

Prepare hardware briefs, use the Ohmbo MCP from Claude Code, and continue on [Ohmbo](https://ohmbo.com/) for the complete product experience.

## Install

In Claude Code 2.1.275 or later:

```
/plugin install ohmbo --marketplace ohmbo-Official/ohmbo-plugin
```

## Account and authentication

The bundled production MCP (`https://mcp.ohmbo.com/mcp`) uses OAuth 2.1. Claude Code opens the Ohmbo website for login and consent; no API key is stored in the plugin or pasted into chat. Authorized MCP jobs appear under [Agent designs](https://ohmbo.com/dashboard/mcp-designs), and tool results include the matching website URL.

Running tasks through MCP or the API is part of the paid workspace plans listed on [pricing](https://ohmbo.com/pricing); the brief and service skills work without an account. Creating or revising a design consumes the account's work credits and backend compute.

Ohmbo also provides [Developer API v1](https://ohmbo.com/docs/api), **Compatible with OpenAI SDKs** for the tested models, Responses, and Chat Completions subset. Create and revoke `sk-ohmbo-live-...` or `sk-ohmbo-test-...` keys in [Developer settings](https://ohmbo.com/settings/apikeys). MCP OAuth, website work, and API keys use the same Ohmbo account and compute ledger in each environment.

## What it does

- `ohmbo-services`: explain Ohmbo's services and choose a starting point.
- `ohmbo-brief`: prepare a copyable product, PCB, or prototype brief. Nothing is sent to Ohmbo; you paste it on the website.
- `ohmbo-continue`: find results, pricing, or contact pages, and check MCP jobs with the user's authorization.

Ohmbo MCP and Developer API v1 currently create and track hosted PCB jobs. A visible Agent or API job is not automatically an editable Studio project. Broader product definition, firmware, simulation, enclosure and appearance work, physical prototype services, orders, pricing, and complete result viewing continue on the website.

## Privacy and support

[Privacy policy](https://ohmbo.com/privacy) · [Terms](https://ohmbo.com/terms) · [founder@ohmbo.com](mailto:founder@ohmbo.com)

## Local development

Start with `claude --plugin-dir /absolute/path/to/ohmbo-plugin`, and restart or reload Claude Code after changes. Try a service question, a hardware brief, and an explicit PCB creation request. For the creation flow, complete browser consent, verify the job from Claude Code, then open the returned Ohmbo page.

## License

The MIT License applies only to the files in this repository. The service running at `ohmbo.com` and `mcp.ohmbo.com` remains proprietary Ohmbo SaaS and is not made open source by this repository.
