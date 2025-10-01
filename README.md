# EZPrompt Library - Prompts Collection

This folder contains individual prompt JSON files that are ready to be uploaded to the [ezprompt-library](https://github.com/Master0fFate/ezprompt-library) repository.

## Structure

Each file is a standalone prompt with the following schema:

```json
{
    "id": 1,
    "title": "Prompt Title",
    "description": "Brief description",
    "category": "Category Name",
    "prompt": "Full prompt template with [PLACEHOLDERS]",
    "example": "Concrete usage example",
    "tags": ["tag1", "tag2", "tag3"],
    "favorite": false,
    "custom": false
}
```

## Upload to GitHub

To contribute prompt to the community library:

1. Fork https://github.com/Master0fFate/ezprompt-library
2. Upload JSON files to the `prompts/` folder
3. Create a Pull Request
4. Once merged, they'll be instantly available to all users!

## Creating New Prompts

Use the **JSON Prompt Builder** in the EZPrompt Studio application to create new prompts. It will generate properly formatted JSON files ready for upload.

## Notes

- Each file must be valid JSON
- The `id` field is auto-generated (timestamp-based)
- Files are named after their title (lowercase, hyphenated)
- `favorite` is always `false` for new prompts
- `custom` is `false` for community prompts, `true` for local-only
