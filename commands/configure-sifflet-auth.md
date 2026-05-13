---
name: configure-sifflet-auth
description: Set up Sifflet authentication for Cursor and Monitors as Code.
---

# Configure Sifflet Authentication

Create an API token in Sifflet first: [Generate an API token](https://docs.siffletdata.com/docs/generate-an-api-token).

Then run:

```bash
sifflet configure
```

Reload Cursor after configuration so the Sifflet MCP server can use the new credentials.

## Verify

- Run `sifflet status`.
- Ask Agent to search the Sifflet catalog.
- For Monitors as Code, run `sifflet code workspace plan --file workspace.yaml`.

Do not commit API tokens or local Sifflet configuration files.
