# Top-Level Upwork AI Agent

A modular AI automation system designed to assist with Upwork-related workflow tasks using n8n.

The system can coordinate multiple specialized workflows for application generation, proposal creation, documentation, and related automation tasks.

## Architecture

```text
                    Upwork AI Agent
                          │
          ┌───────────────┼───────────────┐
          ↓               ↓               ↓
 Application Copy   Google Proposal   Mermaid Code
          │               │               │
          └───────────────┼───────────────┘
                          ↓
                    Final Output
```

## Included Modules

### 01 — Generate Application Copy

Generates customized application/proposal text based on a project description.

### 02 — Generate Google Doc Proposal

Creates a structured proposal and sends it to Google Docs.

### 03 — Generate Mermaid Code

Generates Mermaid diagrams for workflow and process visualization.

### 04 — Top-Level Agent

Coordinates the overall workflow and determines which specialized process should be used.

## Features

* Modular workflow architecture
* AI-powered decision making
* Proposal generation
* Application copy generation
* Google Docs integration
* Mermaid diagram generation
* Reusable components

## Requirements

* n8n
* AI provider
* Google credentials for Google Docs functionality
* Required credentials for any additional integrations

## Project Structure

```text
07-upwork-ai-agent/
│
├── README.md
├── setup.md
│
├── 01-generate-application-copy/
│   ├── workflow.json
│   └── README.md
│
├── 02-generate-google-doc-proposal/
│   ├── workflow.json
│   └── README.md
│
├── 03-generate-mermaid-code/
│   ├── workflow.json
│   └── README.md
│
└── 04-top-level-upwork-ai-agent/
    ├── workflow.json
    └── README.md
```

## Setup

See [`setup.md`](setup.md).

Each specialized workflow can also be configured independently.

## Customization

The system can be extended with additional modules such as:

* Job filtering
* Lead scoring
* Proposal analysis
* Client research
* CRM integration
* Email notifications
* Database storage

## License

See the root `LICENSE` file.
