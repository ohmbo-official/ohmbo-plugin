# Ohmbo plugin

[Ohmbo](https://ohmbo.com/) is a one-stop hardware development platform for the whole hardware journey: requirements and architecture, electronics, firmware, simulation, 3D structure and enclosure, prototypes and measured test, in one project. This plugin brings that project into Claude Code: plan a product, prepare a brief, start and follow design work through the Ohmbo MCP, and continue in the full workspace on ohmbo.com.

## Install

In Claude Code 2.1.275 or later:

```
/plugin install ohmbo --marketplace ohmbo-Official/ohmbo-plugin
```

## Account and authentication

The bundled production MCP (`https://mcp.ohmbo.com/mcp`) uses OAuth 2.1. Claude Code opens the Ohmbo website for login and consent; no API key is stored in the plugin or pasted into chat. Authorized MCP jobs appear under [Agent designs](https://ohmbo.com/dashboard/mcp-designs), and tool results include the matching website URL.

You can start with the Free plan, which needs no subscription and includes one-time trial work credits; other plans and what they include are on [pricing](https://ohmbo.com/pricing). Creating or revising a design uses the account's work credits. The brief and service skills work without an account.

Ohmbo also provides [Developer API v1](https://ohmbo.com/docs/api), **Compatible with OpenAI SDKs** for the tested models, Responses, and Chat Completions subset. Create and revoke `sk-ohmbo-live-...` or `sk-ohmbo-test-...` keys in [Developer settings](https://ohmbo.com/settings/apikeys). MCP OAuth, website work, and API keys use the same Ohmbo account and compute ledger in each environment.

## What it does

- `ohmbo-services`: explain Ohmbo's services and choose a starting point.
- `ohmbo-brief`: prepare a copyable product, design, or prototype brief. Nothing is sent to Ohmbo; you paste it on the website.
- `ohmbo-continue`: find results, pricing, or contact pages, and start, revise and follow MCP design jobs with the user's authorization.

The MCP tools create and revise designs from plain language, report job status, list and cancel jobs, discover capabilities and return artifact metadata. Jobs run asynchronously and appear under Agent designs; the website workspace holds the full project, visual review, released results, quotes and orders.

## Privacy and support

[Privacy policy](https://ohmbo.com/privacy) · [Terms](https://ohmbo.com/terms) · [founder@ohmbo.com](mailto:founder@ohmbo.com)

## Local development

Start with `claude --plugin-dir /absolute/path/to/ohmbo-plugin`, and restart or reload Claude Code after changes. Try a service question, a hardware brief, and an explicit PCB creation request. For the creation flow, complete browser consent, verify the job from Claude Code, then open the returned Ohmbo page.

## License

The MIT License applies only to the files in this repository. The service running at `ohmbo.com` and `mcp.ohmbo.com` remains proprietary Ohmbo SaaS and is not made open source by this repository.
