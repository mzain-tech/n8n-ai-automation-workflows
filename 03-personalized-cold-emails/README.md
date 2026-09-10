# Personalized Cold Emails

An AI-powered n8n workflow for generating personalized cold emails from structured prospect information.

## Features

* AI-generated email personalization
* Prospect-specific messaging
* Company research inputs
* Custom prompts
* Structured email output
* Scalable outreach preparation

## Workflow Overview

```text
Lead Data
    ↓
Prepare Prospect Information
    ↓
AI Personalization
    ↓
Generate Email
    ↓
Validate / Format
    ↓
Email Output
```

## Example Input

```json
{
  "name": "John Smith",
  "company": "Example Company",
  "role": "Marketing Director",
  "website": "https://example.com"
}
```

## Use Cases

* B2B outreach
* Agency prospecting
* Sales campaigns
* Partnership outreach
* Lead nurturing

## Requirements

* n8n
* AI provider
* Prospect data
* Optional email platform

## Prompt Customization

The `prompts.md` file contains the prompts used by the workflow.

Modify them according to your target audience and offer.

## Setup

See [`setup.md`](setup.md).
