# dayNumber_ MCP

dayNumber_ is public proof-of-work logging for founders. Log your daily build journey via MCP, query your history, get insights; your agent keeps your streak alive. A few minutes a day turns your journey into a public record that investors, partners, and future hires can actually read.

This repository is the public descriptor for the dayNumber_ MCP server. It holds configuration and registry files only. The server itself is hosted remotely, and there is no server source code here.

## Connect

- **MCP endpoint:** https://mcp.daynumber.io/mcp (remote, Streamable HTTP)
- **Connect page:** https://daynumber.io/connect
- **Auth:** OAuth 2.1, with an API-key fallback
- **Registry name:** `io.github.magicjordan33/daynumber`

## Add it to your client

For any MCP client that takes a remote `mcpServers` config block:

```json
{
  "mcpServers": {
    "daynumber": {
      "url": "https://mcp.daynumber.io/mcp"
    }
  }
}
```

The same block ships in this repo as [`mcp.json`](mcp.json), and [`plugin.json`](plugin.json) packages it for plugin marketplaces.

## What you can do with it

Log what you shipped today, read back your full history, and get insights from your own log. Connected through your agent, dayNumber_ keeps the streak alive: your agent can see where you left off and help you log today.

## Descriptor files

- `server.json` — Official MCP Registry descriptor (name `io.github.magicjordan33/daynumber`)
- `glama.json` — Glama maintainer claim file
- `plugin.json` — plugin manifest (Cursor Marketplace shape), pointing at the remote endpoint
- `mcp.json` — remote `mcpServers` config block

## Links

- Website: https://daynumber.io
- Connect: https://daynumber.io/connect
