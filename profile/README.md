# Dataville

**One API for the external data your AI applications need: Wikipedia, SEC EDGAR, arXiv, the US Census and more, through REST, SQL and a hosted MCP server.**

Every source returns the same JSON shape with its source URL, license and attribution, so you can cite what you show and combine sources without writing a new integration for each.

[Website](https://dataville.com) · [Docs](https://docs.dataville.com) · [Get a free API key](https://app.dataville.com/api-keys) · [MCP server](https://github.com/datavilleorg/dataville-mcp)

### Try it in 30 seconds

```bash
curl "https://api.dataville.com/edgar/AAPL"      # Apple's latest SEC filing and financials
curl "https://api.dataville.com/wiki/Nvidia"     # Wikipedia article, with source and license
```

Or give your agent the whole catalog. Dataville is in the [Official MCP Registry](https://registry.modelcontextprotocol.io/) as `com.dataville/dataville-mcp`:

```bash
claude mcp add --transport http dataville https://api.dataville.com/mcp
```

### Repositories

| | |
|---|---|
| [**dataville-mcp**](https://github.com/datavilleorg/dataville-mcp) | MCP server for Claude, Cursor, VS Code and other MCP clients (hosted or `npx`) |
| [**dataville-wikimedia**](https://github.com/datavilleorg/dataville-wikimedia) | Build with Wikimedia data: fresh, source-linked Wikipedia articles |
| [**dataville-sec-edgar**](https://github.com/datavilleorg/dataville-sec-edgar) | Build with SEC EDGAR: 10-K, 10-Q and 8-K filings, XBRL financials, insider trades |
| [**company-intelligence-agent**](https://github.com/datavilleorg/company-intelligence-agent) | Research a company from Wikimedia context and SEC disclosures, every claim source-linked |
| [**dataville-news-sentiment-tracker**](https://github.com/datavilleorg/dataville-news-sentiment-tracker) | Sentiment and political leaning across 13M news articles |

### Learn more

- [Quickstart: API](https://docs.dataville.com/quickstart) and [Quickstart: Claude](https://docs.dataville.com/quickstart-claude)
- [Data sources](https://docs.dataville.com/data-sources): every source, how to search it and its license
- [Guides](https://docs.dataville.com/guides/overview): filings watchlists, competitor scans, underwriting checks and more

Questions: [support@dataville.com](mailto:support@dataville.com)
