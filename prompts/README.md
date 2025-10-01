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

## Files in this folder

- `rest-api-development-with-authentication.json` - REST API with JWT auth
- `advanced-algorithm-optimization.json` - Algorithm optimization and analysis
- `comprehensive-code-review.json` - Code review with SOLID principles
- `database-schema-design.json` - Database schema design
- `unit-testing-suite.json` - Unit testing with mocking
- `security-audit.json` - Security audit with OWASP Top 10
- `api-documentation.json` - API documentation generation
- `debugging-assistant.json` - Systematic debugging
- `async-programming.json` - Async patterns and error handling
- `design-pattern-implementation.json` - Design pattern implementation
- `react-component.json` - React component with TypeScript
- `microservices-architecture.json` - Microservices design
- `graphql-api.json` - GraphQL API with resolvers
- `ci-cd-pipeline.json` - CI/CD pipeline setup
- `performance-optimization.json` - Performance analysis
- `react-native-mobile-app.json` - React Native app
- `ml-model-integration.json` - ML model integration
- `websocket-real-time.json` - WebSocket real-time features
- `serverless-functions.json` - Serverless functions
- `data-pipeline-etl.json` - Data pipeline ETL

## Upload to GitHub

To contribute these prompts to the community library:

1. Fork https://github.com/Master0fFate/ezprompt-library
2. Upload these JSON files to the `prompts/` folder
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
