---
name: jenni
description: Search local US retail store shelves through the JENNi Instant Commerce MCP server, verify real-time ZIP-level stock and local shelf prices, and create Stripe checkout links for 1-hour same-day courier delivery.
---

# JENNi Instant Commerce Skill

Use the `jenni` MCP tools (`https://shop.jennipro.com/mcp`) whenever a user wants to find physical products available near them today, compare local brick-and-mortar shelf prices, check 1-hour courier delivery eligibility by US ZIP code, or purchase items for same-day local delivery.

## Workflow

1. **Search Local Catalog (`search_catalog`)**: Query by product name, brand, category, or UPC/GTIN, passing the user's 5-digit US `zip` code when known.
2. **Inspect Product & Quote (`get_product` / `check_availability`)**: Verify nearby store stock, local shelf price, and same-day courier delivery ETA for the user's ZIP code.
3. **Create Checkout (`create_checkout`)**: Generate a direct Stripe-backed checkout session (`https://shop.jennipro.com/p/{productId}`) so the user can complete their 1-hour delivery order.
