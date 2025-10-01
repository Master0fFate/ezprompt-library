# Contributing to EZPrompt Cookbook (JSON)

Thank you for your interest in contributing to the EZPrompt Cookbook! This guide will help you add your own prompt templates to the collection.

## How to Add a New Prompt

### 1. What is this?

- A repository of prompts in a JSON format. (Currently used to be loaded on a website)

### 2. Understand the Prompt Structure

Each prompt entry in the JSON follows this structure:

```json
{
    "id": 1,
    "title": "Your Prompt Title",
    "description": "Brief description of what this prompt does",
    "category": "Category Name",
    "prompt": "The actual prompt template with [PLACEHOLDERS]",
    "example": "A concrete example of how to use this prompt",
    "tags": ["tag1", "tag2", "tag3"],
    "favorite": false,
    "custom": false
}
```

### 3. Field Descriptions

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `id` | Number | ✅ | Unique identifier (use next available number) |
| `title` | String | ✅ | Concise, descriptive title for your prompt |
| `description` | String | ✅ | One-line summary of the prompt's purpose |
| `category` | String | ✅ | Choose from existing or create new category* |
| `prompt` | String | ✅ | The full prompt template with `[PLACEHOLDERS]` for user input |
| `example` | String | ✅ | A real-world example showing how to use the prompt |
| `tags` | Array | ✅ | 3-7 relevant keywords for searchability |
| `favorite` | Boolean | ✅ | Always set to `false` for new prompts |
| `custom` | Boolean | ✅ | Always set to `false` for contributed prompts |

**Default Categories:**
- API Design
- Optimization
- Code Review
- Architecture
- Testing
- Security
- Documentation
- Debugging
- Code Generation
- DevOps

### 4. Prompt Writing Best Practices

**Good prompts should:**
- ✅ Use `[PLACEHOLDERS]` for user-specific information
- ✅ Be well-structured with clear sections
- ✅ Include specific requirements and deliverables
- ✅ Specify expected output format
- ✅ Be reusable across different projects
- ✅ Follow a consistent template structure

**Example of a well-structured prompt:**

```
Create a [TYPE] for [PURPOSE]:

Technical Stack:
- Language/Framework: [SPECIFY]
- Database: [SPECIFY]

Requirements:
1. [Requirement 1]
2. [Requirement 2]
3. [Requirement 3]

Please Provide:
1. Clean, production-ready code
2. Comprehensive error handling
3. Usage examples
```

**Example:**

```javascript
{
    id: 21,
    title: 'GraphQL Resolver Implementation',
    description: 'Generate GraphQL resolvers with database integration and caching',
    category: 'API Design',
    prompt: 'Create GraphQL resolvers for [ENTITY] with the following requirements:\n\nSchema:\n[PASTE GRAPHQL SCHEMA]\n\nRequirements:\n1. Database integration with [DATABASE]\n2. Efficient data loading (DataLoader pattern)\n3. Authentication and authorization\n4. Error handling\n5. Caching strategy\n\nProvide complete resolver implementation with comments.',
    example: 'Create GraphQL resolvers for a User entity with PostgreSQL, including authentication',
    tags: ['graphql', 'api', 'resolvers', 'database', 'caching'],
    favorite: false,
    custom: false
}
```


### 5. Submit Your Contribution

1. Commit your changes:
```bash
git add prompt.json
git commit -m "Add [Your Prompt Title] prompt template"
```

2. Push to your fork:
```bash
git push origin main
```

3. Create a Pull Request:
   - Go to the original repository
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill in the PR template:
     - **Title**: `Add: [Your Prompt Title]`
     - **Description**: Explain what your prompt does and why it's useful
     - **Category**: Mention the category
     - **Testing**: Confirm you tested it in the browser

### 6. PR Review Checklist

Before submitting, ensure:

- [ ] Prompt follows the JSON structure exactly
- [ ] `id` is unique and sequential
- [ ] All required fields are present
- [ ] Prompt uses `[PLACEHOLDERS]` appropriately
- [ ] Example is concrete and helpful
- [ ] Tags are relevant and lowercase
- [ ] No typos or grammatical errors
- [ ] JSON syntax is valid (no trailing commas, proper quotes)
- [ ] Tested in browser successfully

## Tips for Great Prompts

1. **Be Specific**: Include concrete requirements and deliverables
2. **Use Structure**: Organize with clear sections and bullet points
3. **Add Context**: Help LLMs understand the use case
4. **Include Examples**: Show a real-world application
5. **Think Reusability**: Make it flexible with placeholders
6. **Quality Over Quantity**: One excellent prompt > multiple mediocre ones

## Need Help?

- 📧 Need help with JSON? Check the existing prompts for reference

## Code of Conduct

- Be respectful and constructive
- Focus on high-quality, useful prompts
- Help review others' contributions
- Keep prompts professional and appropriate

---

Thank you for contributing! Your prompts help developers work more efficiently with AI Models.
