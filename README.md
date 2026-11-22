# Amazon FBA Inventory & Replenishment Dashboard (demo)

A self-contained, single-file operating dashboard for an Amazon FBA catalog, built
with Claude Code from live Seller Central data. **This is a de-identified demo** — all
real brand, product, and account data has been replaced with placeholder values.

**Live page:** https://kitbrianhernandez-ai.github.io/inventory-dashboard/

## What it shows

- **Replenishment Plan** — per-SKU Available, Inbound, Total, **sales velocity**, an
  **editable forecast** field, Days of cover, Reorder point, Stock-out date, Order
  quantity and Order status — all recomputing live as you adjust the forecast.
- **Inventory & Replenishment** — pool composition, days-of-cover and projected
  stock-out charts.
- **Warehouse / Shipments / Stock Level** — inbound and warehouse-staged units.
- **Sales & Traffic** — sessions, conversion and revenue by product.
- **Overview** — headline KPIs across replenishment, sales and the warehouse.

## How it's built

In production, Claude Code pulls current FBA inventory, Business Report and shipment
data from Seller Central (no manual exports), computes the replenishment math, and
rebuilds this HTML. Nothing is pushed back to Amazon — the dashboard is read-only
reporting for human review.

_Single file — just open `index.html` in a browser._
