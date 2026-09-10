# Setup Guide — Generate Google Doc Proposal

## 1. Import Workflow

Import:

```text
workflow.json
```

into n8n.

## 2. Configure AI Credentials

Configure the AI provider used by the workflow.

## 3. Configure Google Credentials

Connect your Google account through n8n OAuth credentials.

Grant the permissions required by the Google Docs nodes.

## 4. Configure Proposal Input

Provide information such as:

```text
Project title
Client requirements
Scope
Deliverables
Timeline
Applicant/company information
```

## 5. Configure Document

Set the Google Docs destination according to your workflow.

Depending on the implementation, configure:

* Document ID
* Folder
* Document title
* Content

## 6. Test

Run the workflow with a test project.

Verify:

* Proposal content
* Formatting
* Document creation
* Correct Google account
* Correct destination

## Troubleshooting

### Google authentication error

Reconnect the Google OAuth credential.

### Document not created

Check Google Docs node configuration and permissions.

### Poor proposal

Improve the project input and AI prompt.
