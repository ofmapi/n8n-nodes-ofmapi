# OnlyFans API automation with n8n (OFMAPI)

Automate OnlyFans messaging, fan management, and earnings reporting in n8n
with the OFMAPI OnlyFans API. Everything works today through n8n's built-in
**HTTP Request** node (Bearer token) and **Webhook** node (signed inbound
events). A dedicated community node is planned.

**Status: community node planned, not yet on npm.** `n8n-nodes-ofmapi` is
not published, so it cannot be installed from n8n's Community Nodes panel
yet.

## Use the OnlyFans API from n8n today

The guide covers requests, webhook signature verification, and an auto-reply
flow that answers new fan messages:

https://ofmapi.com/docs/integrations/n8n

Quick shape of a request node:

- Method `GET`, URL `https://api.ofmapi.com/v1/accounts`
- Authentication: Header Auth, name `Authorization`, value `Bearer ofmapi_...`

Common workflows:

- New OnlyFans message (webhook) → classify with an LLM → reply through
  `POST /v1/accounts/{account_id}/messages`
- New subscriber → add to a CRM or spreadsheet
- Daily earnings summary → Slack, Telegram, or email

## What OFMAPI is

An independent, unofficial OnlyFans API for agencies and developers: typed
REST endpoints, signed webhooks, and a hosted MCP server (174 tools) for
Claude, ChatGPT, Cursor, and VS Code. Free during the public Beta; no card
required; documented usage limits apply. There is no official OnlyFans
developer API.

- Website: https://ofmapi.com
- Documentation: https://ofmapi.com/docs
- Interactive API reference (no login): https://ofmapi.com/docs/api
- Zapier guide: https://ofmapi.com/docs/integrations/zapier
- Status: https://ofmapi.com/status
- Contact and support: https://ofmapi.com/contact

## Roadmap

This repository will hold the community node source when it is published.
Watch the repository or the changelog at https://ofmapi.com/changelog.

## License

MIT. See [LICENSE](LICENSE).

---

OFMAPI is an independent organisation, not affiliated with OnlyFans.com or
Fenix International Limited. "OnlyFans" is a registered trademark of Fenix
International Limited.
