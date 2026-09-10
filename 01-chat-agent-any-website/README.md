# Chat Agent for Any Website

An AI-powered website chat agent built with n8n. The workflow can receive visitor messages, process them with an AI model, maintain conversational context, and return an intelligent response.

## Features

* AI-powered website chat
* Natural-language conversation
* Conversation memory
* Custom system instructions
* Automated response generation
* Webhook-based communication
* Easy integration with websites
* Can be customized for customer support, lead qualification, FAQs, and sales

## Workflow Overview

```text
Website Chat
     ↓
Webhook
     ↓
Process User Message
     ↓
AI Agent
     ↓
Memory / Context
     ↓
Generate Response
     ↓
Return Response
```

## Use Cases

* Customer support
* Lead qualification
* FAQ assistants
* Product assistants
* Service business chatbots
* Appointment assistants
* Website sales assistants

## Requirements

* n8n
* An AI model/API supported by your workflow
* A website or frontend capable of sending HTTP requests
* Required API credentials

## Installation

1. Open your n8n instance.
2. Import `workflow.json`.
3. Configure the required credentials.
4. Review the AI Agent instructions.
5. Configure the webhook endpoint.
6. Activate the workflow.
7. Connect your website chat interface to the webhook.

See [`setup.md`](setup.md) for detailed configuration instructions.

## Customization

You can customize:

* AI system prompt
* Business information
* Conversation memory
* Response format
* Lead qualification questions
* Website branding
* Model configuration

## Security

Do not expose API keys inside frontend JavaScript.

Use n8n credentials or environment variables for sensitive information.

## License

This project is provided for educational and automation purposes. See the root `LICENSE` file for license information.
