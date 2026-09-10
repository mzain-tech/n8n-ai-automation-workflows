# LinkedIn Lead Scraper

An n8n automation workflow designed to collect and structure publicly available lead information for prospecting and business research.

## Features

* Lead data collection
* Lead information extraction
* Structured output
* Data cleaning
* Prospecting automation
* Export-ready lead records
* AI-assisted lead processing

## Workflow Overview

```text
Lead Source
    ↓
Collect Lead Data
    ↓
Extract Fields
    ↓
Clean / Validate Data
    ↓
AI Processing
    ↓
Structured Lead Output
```

## Typical Lead Fields

Depending on the source, the workflow can process:

* Name
* Job title
* Company
* Profile URL
* Location
* Industry
* Website
* Contact information when legitimately available

## Use Cases

* B2B prospecting
* Sales research
* Lead list preparation
* Market research
* CRM preparation
* Outreach preparation

## Requirements

* n8n
* Required data source
* AI provider if enabled
* Optional spreadsheet/database/CRM

## Setup

Import `workflow.json` into n8n and configure the required source and credentials.

See [`setup.md`](setup.md).

## Important

Use the workflow only with data and sources that you are authorized to access. Respect applicable website terms, privacy requirements, and rate limits.
