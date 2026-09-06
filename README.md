# n8n and the OFMAPI OnlyFans API

**Status: community node planned, not yet on npm.** `n8n-nodes-ofmapi` is
not published, so it cannot be installed from n8n's Community Nodes panel
yet.

## Use OFMAPI from n8n today

Everything works through n8n's built-in **HTTP Request** node with a Bearer
token, and inbound events arrive through n8n's **Webhook** node. The guide
covers both, including signature verification and an auto-reply flow:

https://ofmapi.com/docs/integrations/n8n

Quick shape of a request node:

- Method `GET`, URL `https://api.ofmapi.com/v1/accounts`
- Authentication: Header Auth, name `Authorization`, value `Bearer ofmapi_...`

## What OFMAPI is

A typed REST API over OnlyFans for agencies and developers, plus a hosted
MCP server (174 tools) for Claude, ChatGPT, Cursor, and VS Code. Free
during the public Beta; no card required; documented usage limits apply.

- Website: https://ofmapi.com
- Documentation: https://ofmapi.com/docs
- Interactive API reference (no login): https://ofmapi.com/docs/api
- Zapier guide: https://ofmapi.com/docs/integrations/zapier
- Status: https://ofmapi.com/status

## Roadmap

This repository will hold the community node source when it is published.
Watch the repository or the changelog at https://ofmapi.com/changelog.

## License

MIT. See [LICENSE](LICENSE).

---

OFMAPI is an independent organisation, not affiliated with OnlyFans.com or
Fenix International Limited. "OnlyFans" is a registered trademark of Fenix
International Limited.
