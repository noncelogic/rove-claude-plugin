# Rove — Claude plugin

Rove is the supervised browser for AI agents. Your agent drives a real hosted
browser; the moment a step needs a person — a login, a CAPTCHA, a payment, a
judgement call — control hands to a human in a live viewer, then hands back.
Persistent profiles keep your agent signed in between runs, extraction returns
structured data instead of page dumps, and every session leaves a full audit
trail you can replay.

This repository is the plugin bundle for the
[Claude connector directory](https://claude.com/docs/connectors): it points
Claude at Rove's hosted MCP server — the same endpoint as the Rove connector —
and packages four example prompts as commands.

## Install

Add this repository as a Claude plugin, or connect the MCP server directly:

- **Server URL:** `https://api.roveapi.com/mcp`
- **Transport:** streamable HTTP, OAuth 2.0 sign-in

## Example commands

- `/supervised-signup` — sign up on a site in a supervised session; a human
  takes over for the password and verification steps.
- `/extract-event-schema` — extract a structured schema from a page.
- `/read-page-visually` — read a page the way a person sees it when its text
  tree is unreadable.
- `/form-to-payment` — fill a checkout form and hand over at the payment step.

## Links

- Documentation: https://roveapi.com/docs
- MCP guide: https://roveapi.com/docs/mcp
- Supervised sessions: https://roveapi.com/docs/supervised
- Privacy policy: https://roveapi.com/privacy
- Support: jg@noncelogic.com

## License

MIT
