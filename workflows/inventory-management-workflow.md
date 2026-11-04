# Marketplace Inventory Management Workflow

A practical workflow for keeping inventory data consistent across an eCommerce operation.

## 1. Establish a source of truth
- Choose the system that owns available-to-sell inventory.
- Maintain a consistent SKU across connected systems, or document each mapping.
- Define who can edit quantities and product status.

## 2. Prepare the catalog
- [ ] Match each marketplace listing to the correct internal SKU.
- [ ] Review duplicate SKUs, bundles, kits, and variations.
- [ ] Confirm fulfillment method, warehouse, lead time, and safety stock rules.
- [ ] Document products that should not sync to particular channels.

## 3. Configure synchronization
- Set the correct inventory source and update frequency.
- Map available quantity, stock status, and fulfillment fields.
- Use a safety buffer when appropriate to reduce overselling risk.
- Confirm how cancellations, returns, and reserved stock affect available quantity.

## 4. Test before scaling
- Test a small group of SKUs first.
- Compare source quantities with each connected channel.
- Confirm that stock decreases after an order and increases only when the workflow permits.
- Check how zero stock, discontinued items, and sync errors are handled.

## 5. Monitor exceptions
Review:
- Quantity mismatches
- Failed or delayed sync jobs
- Unmapped SKUs
- Unexpected out-of-stock listings
- Duplicate orders or fulfillment conflicts

Record the SKU, channel, time, expected value, actual value, and corrective action.

## 6. Reconcile regularly
- Compare channel quantities with the inventory source.
- Investigate recurring differences rather than repeatedly correcting symptoms.
- Keep a change log for mappings and sync rules.

**Important:** Exact settings depend on the marketplace, integration tool, and fulfillment model. Test changes in a controlled scope and follow each platform's current documentation.
