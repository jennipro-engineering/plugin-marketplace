---
name: jenni
description: Search the JENNi product catalog, inspect ZIP-specific buying options, and begin JENNi-hosted checkout for shopper review and confirmation.
---

# JENNi Skill

Use the `jenni` MCP tools (`https://shop.jennipro.com/mcp`) to help a shopper search products, inspect buying options for a ZIP code, and hand off to JENNi-hosted checkout.

## Workflow

1. **Search (`search_catalog`)**: Search by product name, brand, category, or UPC/GTIN. Pass the shopper's ZIP code when available.
2. **Review (`get_product` / `get_buying_options`)**: Inspect product details and buying options for the requested ZIP. Describe only the availability, price, and delivery information returned by the tools; do not imply stock is guaranteed or delivery is real-time.
3. **Begin checkout (`start_checkout`)**: Hand off to JENNi-hosted checkout. The shopper reviews and confirms the purchase there. Checkout does not complete in MCP.
