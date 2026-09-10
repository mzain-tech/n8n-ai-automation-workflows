# Google Maps Scraper — No API

An n8n workflow for collecting publicly available business information from Google Maps-related search results without requiring a direct Google Maps API integration.

## Features

* Business search automation
* Business information extraction
* Structured lead data
* Data cleaning
* Lead qualification
* Export-ready output

## Workflow Overview

```text
Search Query
     ↓
Collect Results
     ↓
Extract Business Data
     ↓
Clean Data
     ↓
Optional AI Processing
     ↓
Structured Output
```

## Possible Data Fields

* Business name
* Category
* Address
* Phone
* Website
* Rating
* Review count
* Maps URL

Actual fields depend on the source and workflow implementation.

## Use Cases

* Local business prospecting
* Agency lead generation
* Market research
* Local SEO research
* Business directory preparation

## Requirements

* n8n
* Compatible data collection method
* Optional AI provider
* Optional spreadsheet/database

## Setup

See [`setup.md`](setup.md).

## Important

Web scraping can be restricted by website terms and technical controls. Use authorized methods and respect applicable rules and rate limits.
