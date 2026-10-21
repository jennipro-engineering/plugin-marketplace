# JENNi Instant Commerce plugin for Grok Build

Connect Grok Build to [JENNi Instant Commerce](https://shop.jennipro.com) to search 58,900+ GTIN-verified products on local US brick-and-mortar retail shelves, verify real-time ZIP-level availability and pricing, and dispatch 1-hour courier delivery.

## Installation

In Grok Build, open `/plugin`, search for **jenni**, and install. No API key is required.

## What you get

- **MCP server** `jenni` at `https://shop.jennipro.com/mcp` (Streamable HTTP, no API key required).
- **Skill** `jenni`: workflow instructions for searching local retail inventory by US ZIP code, verifying local shelf pricing, and generating instant Stripe checkout links.

### Tools

| Tool | Purpose |
|---|---|
| `search_catalog` | Search GTIN-verified products across 33,000+ local US retail stores with optional `zip` filter |
| `get_product` | Retrieve product details, GTIN/UPC, local shelf price, and instant checkout URL |
| `check_availability` | Verify real-time local store stock and calculate 1-hour courier delivery quote for a US ZIP code |
| `create_checkout` | Create a Stripe-backed checkout session for same-day local courier delivery |

## License

MIT
