# Prosacco Supply Chain Planning Project

## Project Overview

A weekly Production, Sales and Inventory (PSI) planning project for **Prosacco**, covering **October–December 2023 (weeks 39–52)**. It tests whether the production plan can cover customer demand from the Kern warehouse, compares an **Original** plan against a **Delayed** plan, and estimates which customers are affected when stock runs short.

---

## Important Files

| File | Purpose |
|---|---|
| `Prosacco_Original_Data.xlsx` | Raw source data and the original PSI sheets built with `VLOOKUP`. |
| `Prosacco_Supply_Chain_Project.xlsx` | Cleaned model with a scenario switch, dashboard, inventory review and customer-impact analysis. |

---

## Dataset at a Glance

| Item | Value |
|---|---|
| Period | 2023, weeks 39–52 (demand starts in week 40) |
| SKUs | 12 across 7 categories |
| Warehouse | Kern (single warehouse) |
| Order lines | 2,880 |
| Total demand | 109,994 units, about $13.75M order value |
| Customers | 17 |
| Channels | Retail, Ecomm, Major Distributor, D2C, Closeout |
| Countries | United States, Canada, Mexico |
| Opening stock | 18,333 units |
| Planned production | 97,000 units in both scenarios (only the timing differs) |

---

## Both Workbooks

### `Prosacco_Original_Data.xlsx`

| Sheet | Contents |
|---|---|
| Initital Inventory | Opening stock per SKU. |
| Customer Orders | 2,880 order lines with SKU, quantity, channel, customer, sales USD and expected date. |
| Customer Orders (Week) | Order quantity by SKU and week. |
| Production Plan (Original) | Planned production per SKU per week. |
| Production Plan (Delay) | Same plan with delayed production. |
| PSI (Original) / PSI (Delay) | Weekly inventory flow per SKU: initial inventory, production, demand, final inventory. |
| Customer Master | Customer codes, locations and contact details. |

### `Prosacco_Supply_Chain_Project.xlsx`

| Sheet | Contents |
|---|---|
| Dashboard | Key metrics, weekly supply and demand table, and chart. |
| Controls | Scenario switch (`B5`: 1 = Original, 2 = Delayed) and demand multiplier (`B6`). |
| PSI Plan | Weekly opening stock, production, demand, fulfilled, closing stock, shortage and fill rate per SKU. |
| Inventory Review | Stock, weeks of cover and suggested action per SKU. |
| Customer Impact | Estimated shortage exposure per customer. |
| Orders | Cleaned order data with planned demand and shortage share. |
| Products | SKU list with category, warehouse and opening units. |
| Production | Production plans for both scenarios. |
| Source | Notes on data origin and method. |
