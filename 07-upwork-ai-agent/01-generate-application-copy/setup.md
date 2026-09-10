# Setup Guide — Generate Application Copy

## 1. Import

Import:

```text
workflow.json
```

into n8n.

## 2. Provide Job Information

The workflow should receive the project/job description.

Example:

```text
We need an automation developer to build an n8n workflow...
```

## 3. Provide Applicant Information

Add relevant information such as:

* Skills
* Experience
* Projects
* Services
* Relevant achievements

## 4. Configure AI Prompt

Tell the AI to focus only on information relevant to the job.

Avoid unsupported claims.

## 5. Configure Output

Recommended output:

```text
application
```

or:

```text
proposal
```

## 6. Test

Use several different job descriptions and check whether the generated application changes according to the requirements.

## Troubleshooting

### Generic application

Provide more specific applicant information and improve the prompt.

### Incorrect claims

Restrict the AI to supplied applicant information.

### Too much text

Set an explicit maximum length.
