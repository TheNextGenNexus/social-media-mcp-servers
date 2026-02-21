# social-media-mcp-servers

MCP servers for social media, content platforms, and entertainment data — powered by [nexgendata](https://apify.com/nexgendata) on Apify.

## MCP Servers


### [Social & Content MCP Server](./servers/social-content-mcp-server/)

Access Hacker News, Dev.to, IMDB, podcasts, and Eventbrite data through the Model Context Protocol

**Tools:** `get_hackernews_stories`, `get_devto_articles`, `search_imdb`, `search_podcasts`, `search_eventbrite`

**Install:** `npx @nexgendata/social-content-mcp-server`


## Quick Start

Each server can be installed independently:

```bash
# Pick the server you need
npx @nexgendata/<server-name>
```

Then add it to your Claude Desktop or Cline configuration.

## About nexgendata

nexgendata provides 64 data tools on the [Apify platform](https://apify.com/nexgendata), including 15 MCP servers for AI agent integration. Our tools cover social media, business data, web intelligence, finance, e-commerce, and more.

- **Blog:** [thenextgennexus.com](https://thenextgennexus.com)
- **Apify Store:** [apify.com/nexgendata](https://apify.com/nexgendata)
- **RapidAPI:** [rapidapi.com/rubymoonshot](https://rapidapi.com/user/rubymoonshot)

## License

MIT
