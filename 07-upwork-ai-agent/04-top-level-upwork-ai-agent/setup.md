# Setup Guide — Upwork AI Agent

## 1. Requirements

Install or configure:

* n8n
* AI provider
* Google OAuth credentials if using Google Docs
* Any additional integrations required by your workflows

## 2. Import the Specialized Workflows

Import the workflow files from:

```text
01-generate-application-copy/workflow.json
02-generate-google-doc-proposal/workflow.json
03-generate-mermaid-code/workflow.json
04-top-level-upwork-ai-agent/workflow.json
```

## 3. Configure AI Credentials

Configure the AI credentials required by each workflow.

Use n8n's credential system instead of hard-coding API keys.

## 4. Configure Google Docs

If the Google Docs proposal workflow is enabled:

1. Connect your Google account.
2. Configure OAuth credentials.
3. Grant the required permissions.
4. Configure the destination document/folder.

## 5. Configure the Application Generator

Provide:

```text
Job description
Applicant profile
Skills
Experience
Relevant projects
```

The AI should generate content specifically matched to the project.

## 6. Configure the Proposal Generator

Provide:

```text
Client requirements
Project scope
Deliverables
Timeline
Pricing information
Company/applicant information
```

Adjust the fields according to your implementation.

## 7. Configure Mermaid Generator

Provide a process description and generate Mermaid code for documentation or visualization.

## 8. Configure the Top-Level Agent

The top-level agent should determine which specialized workflow is appropriate for the incoming request.

Example routing:

```text
Application request
        ↓
Generate Application Copy

Proposal document request
        ↓
Generate Google Doc Proposal

Diagram request
        ↓
Generate Mermaid Code
```

## 9. Test Each Module Independently

Before testing the complete agent, test each workflow separately.

Recommended order:

```text
01 → 02 → 03 → 04
```

## 10. Test the Complete Agent

Send a realistic request to the top-level workflow.

Verify:

* Correct routing
* Correct workflow execution
* Correct input mapping
* Correct AI output
* Correct final response

## Troubleshooting

### Wrong workflow selected

Improve the routing instructions and define clear conditions.

### Missing input

Make the top-level agent validate required fields before calling a sub-workflow.

### Google Docs failure

Reconnect Google OAuth and verify document permissions.

### AI output is inconsistent

Use structured prompts and clearly define the expected output format.

### Sub-workflow does not execute

Check the n8n workflow ID/reference and confirm the target workflow is available and active.
