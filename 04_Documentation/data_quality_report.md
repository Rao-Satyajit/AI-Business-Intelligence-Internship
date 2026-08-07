# Data Quality Report

## Data Quality Audit

I checked the dataset in Power Query for missing values, errors, duplicate-looking values, and unusual values.

- All checked columns showed 100% valid values.
- No errors or empty values were found.
- Order ID has repeated values. There are 673 distinct Order IDs and 450 unique Order IDs.
- Repeated Order IDs are not necessarily a problem because one order can contain multiple products.
- Sales was checked from lowest to highest and no negative Sales values were found.
- Profit contains some negative values. These can represent orders where the business made a loss, so they should not automatically be removed.
- No obvious invalid or impossible values were found during today's check.
- No data was removed or changed during the audit.

## Planned Fix

No major changes are needed right now because I did not find any actual errors in the data. I will check these values again during the cleaning process and keep the repeated Order IDs and negative Profit values unless I find that they are incorrect.
