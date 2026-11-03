# Social & Content MCP Server

Access Hacker News, Dev.to, IMDB, podcasts, and Eventbrite data through the Model Context Protocol — powered by [nexgendata](https://apify.com/nexgendata?fpr=2ayu9b) on Apify.

## Quick Start

### Using npx (recommended)

```bash
npx @nexgendata/social-content-mcp-server
```

### Install globally

```bash
npm install -g @nexgendata/social-content-mcp-server
```

## Configure with Claude Desktop

Add to your Claude Desktop config (`~/Library/Application Support/Claude/claude_desktop_config.json` on macOS):

```json
{
      "mcpServers": {
            "social-content-mcp-server": {
                  "command": "npx",
                  "args": [
                        "-y",
                        "@nexgendata/social-content-mcp-server"
                  ],
                  "env": {
                        "APIFY_TOKEN": "your-apify-token-optional"
                  }
            }
      }
}
```

## Configure with Cline

Add the same configuration to your Cline MCP settings.

## Available Tools

| Tool | Description |
|------|-------------|
| `get_hackernews_stories` | Get top/new/best stories from Hacker News |
| `get_devto_articles` | Search and retrieve articles from Dev.to |
| `search_imdb` | Search for movies and TV shows on IMDB |
| `search_podcasts` | Search podcast episodes across platforms |
| `search_eventbrite` | Search for events on Eventbrite |


## Environment Variables

| Variable | Required | Description |
|----------|----------|-------------|
| `APIFY_TOKEN` | No | Your Apify API token for authenticated access. Without it, the server uses the public endpoint (rate-limited). |

## How It Works

This MCP server acts as a local stdio bridge to the [nexgendata Apify MCP endpoint](https://nexgendata--social-content-mcp-server.apify.actor/mcp). When you call a tool, it forwards the request to Apify and returns the results.

## Links

- [Apify Store](https://apify.com/nexgendata/social-content-mcp-server?fpr=2ayu9b)
- [GitHub Repository](https://github.com/TheNextGenNexus/social-media-mcp-servers)
- [nexgendata Blog](https://thenextgennexus.com)

## License

MIT
