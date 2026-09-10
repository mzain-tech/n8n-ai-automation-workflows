# Setup Guide — WhatsApp AI Agent

## 1. Requirements

You need:

* n8n
* A supported WhatsApp Business API/provider
* AI API credentials
* Public HTTPS access for webhooks

## 2. Import Workflow

Import:

```text
workflow.json
```

into n8n.

## 3. Configure WhatsApp Credentials

Add your WhatsApp provider credentials to n8n.

Do not hard-code credentials inside the workflow.

## 4. Configure Webhook

Configure the incoming webhook according to your WhatsApp provider.

Make sure the provider can reach your n8n webhook over HTTPS.

## 5. Configure AI Agent

Update the system instructions.

Example:

```text
You are a customer support assistant.

Answer customer questions clearly and briefly.
Use the available business information.
If information is unavailable, do not invent an answer.
```

## 6. Configure Conversation Memory

Use a unique customer identifier to maintain separate conversations.

Example:

```text
phone_number
```

## 7. Configure Outgoing Message

Map the generated AI response to your WhatsApp provider's outgoing message node/API request.

## 8. Test

Send a test WhatsApp message and verify:

```text
Incoming message
→ n8n
→ AI
→ WhatsApp response
```

## 9. Production

After testing, activate the workflow.

Monitor failed executions and API errors.

## Troubleshooting

### Webhook not receiving messages

Check the provider webhook configuration and HTTPS endpoint.

### AI does not respond

Check the AI credentials and node execution.

### Wrong conversation context

Check the customer/session identifier.

### Message sending fails

Verify the WhatsApp provider credentials and recipient/message format.
