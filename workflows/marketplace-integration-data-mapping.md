# Marketplace Integration: Data Mapping Template

Use this template to plan a connection between a catalog, inventory/order system, and one or more sales channels.

## Mapping table

| Business field | Source field | Destination field | Validation rule | Owner / notes |
|---|---|---|---|---|
| Internal SKU |  |  | Must be unique and stable |  |
| Marketplace listing ID |  |  | Preserve channel-specific ID |  |
| Product title |  |  | Follow channel rules |  |
| Brand |  |  | Match verified product data |  |
| GTIN / UPC / EAN |  |  | Validate identifier type and value |  |
| Available quantity |  |  | Define safety stock and update timing |  |
| Price |  |  | Confirm currency and pricing rules |  |
| Fulfillment method |  |  | Map to supported channel values |  |
| Order ID |  |  | Preserve channel reference |  |
| Order status |  |  | Map allowed status values |  |
| Tracking number |  |  | Validate carrier and tracking format |  |

## Integration checklist
- [ ] Identify the authoritative source for product, price, inventory, and orders.
- [ ] Document SKU and listing-ID relationships.
- [ ] Define sync direction and frequency for each field.
- [ ] Decide how conflicts and failed updates are handled.
- [ ] Confirm currency, units, time zones, and status-value mappings.
- [ ] Define retry rules and who receives error notifications.
- [ ] Test new listings, updates, stock changes, orders, cancellations, and tracking.
- [ ] Record test results and obtain approval before scaling.

## Suggested test cases
1. New SKU with complete data
2. Existing SKU title or attribute update
3. Quantity decreases after an order
4. Quantity reaches zero
5. Unmapped SKU
6. Invalid price or missing required attribute
7. Order cancellation
8. Shipment with tracking
9. Temporary connection or API failure
10. Duplicate event or retry

**Safety note:** This is a planning template, not a connector-specific configuration. Confirm supported fields and behavior in the official documentation for the actual integration.
