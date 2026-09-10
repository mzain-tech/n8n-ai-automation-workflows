# Setup Guide — Personalized Cold Emails

## 1. Import Workflow

Import:

```text
workflow.json
```

into your n8n instance.

## 2. Configure AI Credentials

Open the AI node and configure the required credential.

## 3. Prepare Lead Data

Provide structured lead information.

Example:

```json
{
  "name": "John Smith",
  "company": "Example Company",
  "role": "Marketing Director",
  "website": "https://example.com"
}
```

## 4. Configure Prompts

Open:

```text
prompts.md
```

and review the prompts.

Personalize:

* Target industry
* Service
* Tone
* Email length
* Call to action
* Personalization rules

## 5. Recommended Email Structure

The generated email should generally contain:

1. Personalized opening
2. Relevant observation
3. Clear value proposition
4. Short call to action

Avoid unnecessary long paragraphs.

## 6. Test

Start with a small number of leads.

Review generated emails manually before connecting an automated sending system.

## 7. Email Integration

If you connect an email provider, configure its n8n credential and map:

```text
recipient
subject
body
```

## Troubleshooting

### Generic emails

Improve the personalization input and prompt.

### Wrong company information

Validate the source data before sending it to the AI model.

### Emails are too long

Add an explicit word or character limit to the prompt.
