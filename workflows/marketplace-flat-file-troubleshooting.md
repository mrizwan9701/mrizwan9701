# Marketplace Flat-File Troubleshooting Guide

Use this guide when a marketplace bulk upload reports errors or does not update the expected fields.

## 1. Keep a safe working copy
- Download the latest template for the correct marketplace, category, and task.
- Save an untouched original file.
- Work in a separate copy and keep a record of changes.

## 2. Validate the structure
- [ ] Keep required column headers exactly as provided.
- [ ] Do not rename fields or remove required columns.
- [ ] Use the accepted template version and file format.
- [ ] Avoid changing identifiers or formatting unintentionally in spreadsheet software.
- [ ] Check required values and permitted values for each field.

## 3. Check common data errors
- Missing required attributes
- Invalid category or product type
- Incorrect SKU, product ID, or identifier type
- Unsupported variation theme or parent-child relationship
- Invalid date, decimal, unit, or Boolean format
- Duplicate records or conflicting values
- Values exceeding field limits
- Image links that are inaccessible or incorrectly formatted

## 4. Read the processing report
- Find the exact row, field, error code, and message.
- Separate blocking errors from warnings.
- Correct a small batch first and re-upload it.
- Wait for processing to finish before judging the result.
- Recheck the live listing or processing status after a successful upload.

## 5. Avoid risky bulk edits
- Do not overwrite fields you did not intend to change.
- Confirm whether blank cells mean clear, leave unchanged, or invalid for the particular upload type.
- Use a small test batch before a large update.
- Keep a backup and change log.

## 6. Troubleshooting record
For each issue, record:
- Marketplace and upload type
- Template version and date
- SKU or row identifier
- Error message
- Root cause
- Correction made
- Result after reprocessing

**Note:** Error meanings and accepted values differ by marketplace and category. Use the current official template, valid-value definitions, and processing report for the affected upload.
