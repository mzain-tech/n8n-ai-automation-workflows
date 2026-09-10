# Setup Guide — Generate Mermaid Code

## 1. Import

Import:

```text
workflow.json
```

into n8n.

## 2. Configure AI

Add your AI provider credential.

## 3. Provide Description

Give the AI a clear description of the process.

Example:

```text
User submits a form.
n8n receives the form.
The data is validated.
AI analyzes the request.
The result is stored in Google Sheets.
```

## 4. Configure Mermaid Prompt

Tell the AI to return only valid Mermaid code when required.

Example:

```text
Convert the provided process into a Mermaid flowchart.

Return valid Mermaid syntax.
Do not add explanations outside the Mermaid code.
```

## 5. Test

Run several process descriptions and verify the generated Mermaid syntax.

## Troubleshooting

### Invalid Mermaid

Make the prompt stricter and specify the Mermaid diagram type.

### Missing steps

Provide a more detailed process description.

### Incorrect relationships

Describe the order and conditions explicitly.
