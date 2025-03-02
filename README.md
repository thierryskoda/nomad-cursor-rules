# Nomad Project Cursor Rules

This repository contains custom Cursor rules for the Nomad project. These rules help maintain code quality and consistency across the codebase.

## Features

- TypeScript best practices
- React Query conventions
- Zod schema validation patterns
- Supabase integration guidelines
- Design system usage recommendations
- API security checks

## Installation

To use these rules in your Nomad project:

1. Create a `.cursor` directory in your project root if it doesn't exist already
2. Copy the `rules.json` file from this repository into that directory
3. Restart Cursor to apply the rules

```bash
mkdir -p /path/to/your/nomad/project/.cursor
cp .cursor/rules.json /path/to/your/nomad/project/.cursor/
```

## Rule Descriptions

### TypeScript Import Suggestions
Encourages organizing imports alphabetically for better readability.

### Zod Schema Naming Convention
Ensures Zod schemas follow the naming convention of ending with 'Schema'.

### React Query Key Convention
Promotes descriptive and hierarchical query keys for better caching.

### Missing Type Annotations
Identifies functions missing return type annotations.

### Supabase Client Usage
Encourages typed Supabase queries with proper error handling.

### Environment Variable Access
Ensures environment variables are properly validated and have fallbacks.

### Design System Component Usage
Promotes using design system components for consistent UI.

### API Key Security
Flags potential security issues with API keys.

### Commented Code
Identifies commented debug code that should be removed before committing.

### React Query Hook Naming
Ensures React Query hooks follow the 'use' prefix convention.

## Customization

Feel free to modify the rules to better suit your project's specific needs. The `rules.json` file is well-documented and easy to customize.

## Contributing

If you have suggestions for additional rules or improvements to existing ones, please create an issue or pull request.