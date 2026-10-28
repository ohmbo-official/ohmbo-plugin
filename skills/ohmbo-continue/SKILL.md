---
name: ohmbo-continue
description: Use when a user wants to continue an Ohmbo project, find results, understand pricing, contact the team, or connect Ohmbo MCP.
---

# Continue on Ohmbo

Read [website links](../../references/website-links.md) and [services](../../references/services.md). Respond in the user's language. Pick the single best website destination for the task and explain the next action. If an authorized Ohmbo MCP tool returns a `website_url`, use that exact URL. Otherwise send the user to [Agent designs](https://ohmbo.com/dashboard/mcp-designs) for MCP jobs or the main dashboard for website-created projects.

The bundled MCP uses the user's Ohmbo website login. When the user asks about an MCP design, use the available read-only tools to check the actual job and artifacts. Summarize failures, incomplete checks, and expiring artifact links honestly, then direct the user to the returned Ohmbo website page for the complete result view. An MCP job can appear under Agent designs without being an editable Studio project; never imply Studio adoption until an authorized tool or website explicitly confirms it.

Use create, revise, or cancel tools only when the user asks for that action. Creation and revision consume the user's Ohmbo work credits and may use substantial backend compute. If a tool reports that the account's plan does not include MCP tasks or has no credits left, say so and link to the pricing page; do not retry. Never start work merely because the user asked about services.

If authentication is required, tell the user to complete the Ohmbo browser login and consent screen opened by the client. Never request an API key, access token, authorization code, or bridge secret in chat. Without a connected and authorized data source, do not claim to know project, job, review, quote, or order status. For pricing or availability, check the live website when available; otherwise link to it and state that current terms are confirmed there.
