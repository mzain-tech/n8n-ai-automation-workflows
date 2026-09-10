# Setup Guide — LinkedIn Comments + YouTube

## 1. Import

Import:

```text
workflow.json
```

into n8n.

## 2. Configure Content Source

Configure the source used by your workflow.

Provide the required:

* URL
* Post/video identifier
* Search input
* Content text

depending on your implementation.

## 3. Configure AI

Add your AI credentials and configure the model.

## 4. Configure Comment Prompt

A useful instruction can be structured like:

```text
Write a short, natural comment that adds value to the discussion.

Do not repeat the original post.
Do not use generic praise.
Keep the comment conversational.
```

Modify the prompt for your target audience.

## 5. Review Before Publishing

During testing, keep the workflow in a generation/review mode.

Check generated comments before enabling any publishing action.

## 6. Test

Run the workflow with a small number of posts/videos.

Check:

* Content extraction
* AI output
* Comment quality
* Duplicate responses
* Formatting

## Troubleshooting

### Poor comments

Improve the prompt and provide more context to the AI.

### Content extraction fails

Check the source and extraction method.

### Duplicate comments

Add post/video identifiers and maintain a record of processed content.
