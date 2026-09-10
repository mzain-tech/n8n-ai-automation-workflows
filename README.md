# n8n AI Automation Workflows

A collection of reusable n8n workflows for AI agents, lead generation,
web scraping, customer support, cold email personalization, WhatsApp
automation, social media engagement, and Upwork proposal generation.

## Workflows

| Workflow | Description |
|---|---|
| Chat Agent for Any Website | Website chat agent using n8n webhooks and AI |
| LinkedIn Lead Scraper | Collects and processes LinkedIn lead data |
| Personalized Cold Emails | Generates personalized outreach emails using AI |
| Google Maps Scraper | Collects business data from Google Maps without a direct API |
| WhatsApp AI Agent | AI-powered WhatsApp assistant |
| LinkedIn Comments YouTube | Generates or processes LinkedIn and YouTube comments |
| Upwork AI Agent | Generates application copy, proposals, Mermaid code, and complete Upwork workflow |

## Requirements

- n8n Cloud or self-hosted n8n
- Required AI provider API key
- Required Google, Gmail, WhatsApp, LinkedIn, or other credentials
- A webhook URL if the workflow uses a webhook trigger
- Permission to collect and process the data used by the workflow

## How To Use

1. Open the required workflow folder.
2. Read its `README.md` and `setup.md`.
3. Import `workflow.json` into n8n.
4. Create the required credentials in n8n.
5. Replace placeholder values.
6. Test the workflow with sample data.
7. Review the output.
8. Activate the workflow only after testing.

## Security

Do not upload:

- API keys
- Passwords
- OAuth tokens
- Browser cookies
- WhatsApp access tokens
- LinkedIn session data
- Private customer data
- Email lists containing personal information

## Disclaimer

This repository contains automation examples. Users are responsible for
following the terms of service, privacy laws, anti-spam laws, platform
policies, and applicable regulations when using these workflows.
