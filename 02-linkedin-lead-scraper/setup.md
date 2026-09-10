# Setup Guide — LinkedIn Lead Scraper

## 1. Import

Open n8n and import:

```text
workflow.json
```

## 2. Configure the Data Source

Configure the source used by the workflow.

Depending on your implementation, this may be:

* An authorized data provider
* An input file
* A webhook
* A browser/data extraction service

## 3. Configure Lead Fields

Review the fields being extracted.

Recommended structure:

```text
name
job_title
company
profile_url
location
industry
website
```

Only collect fields that are necessary for your intended use.

## 4. Configure AI Processing

If the workflow uses an AI node, configure the required AI credential.

You can use AI to:

* Clean job titles
* Classify industries
* Identify potential decision makers
* Normalize company names
* Score leads

## 5. Configure Output

Connect the output to your preferred destination, such as:

* Google Sheets
* Airtable
* Database
* CRM
* JSON output

## 6. Test

Run the workflow with a small dataset first.

Check:

* Missing fields
* Duplicate leads
* Invalid URLs
* Incorrect company names
* AI classification results

## 7. Production

Use reasonable request rates and avoid unnecessary repeated requests.

Monitor execution history regularly.

## Troubleshooting

### Duplicate leads

Add a unique identifier such as profile URL or email before inserting records.

### Missing fields

Check the source structure and field mapping.

### AI results are inconsistent

Improve the system prompt and provide a strict output format.
