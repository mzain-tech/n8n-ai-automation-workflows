# Setup Guide — Google Maps Scraper

## 1. Import

Import:

```text
workflow.json
```

into n8n.

## 2. Configure Search Input

Provide the search keyword or business category.

Example:

```text
dentists in Lahore
```

or:

```text
real estate agencies in Islamabad
```

## 3. Configure Data Collection

Configure the extraction method used by the workflow.

Review:

* Search URL
* Request settings
* Selectors
* Pagination
* Result limits

## 4. Configure Data Fields

Map the extracted information into a consistent structure.

Example:

```text
business_name
category
address
phone
website
rating
review_count
maps_url
```

## 5. Configure AI Processing

If AI processing is included, it can be used for:

* Lead qualification
* Industry classification
* Business description generation
* Lead scoring

## 6. Configure Output

Recommended destinations include:

* Google Sheets
* Airtable
* PostgreSQL
* CRM
* JSON

## 7. Test

Start with a small search.

Verify that:

* Results are correctly extracted.
* Duplicate businesses are removed.
* URLs are valid.
* Missing fields are handled.

## Troubleshooting

### No results

Check the source structure and search input.

### Missing fields

Inspect the extraction node and update its field mapping.

### Too many requests

Reduce batch size and add appropriate delays.
