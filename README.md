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
2. Copy the rule files from this repository into that directory
3. Restart Cursor to apply the rules

```bash
mkdir -p /path/to/your/nomad/project/.cursor
cp .cursor/*.json /path/to/your/nomad/project/.cursor/
```

## Rule Files

This repository contains multiple rule files:

- `rules.json` - General TypeScript and React rules
- `supabase-rules.json` - Specific rules for Supabase integration
- `design-system-rules.json` - Rules for consistent design system usage

You can use all of these files together or pick the ones that are most relevant to your project.

## Rule Descriptions

### General Rules (rules.json)

#### TypeScript Import Suggestions
Encourages organizing imports alphabetically for better readability.

#### Zod Schema Naming Convention
Ensures Zod schemas follow the naming convention of ending with 'Schema'.

#### React Query Key Convention
Promotes descriptive and hierarchical query keys for better caching.

#### Missing Type Annotations
Identifies functions missing return type annotations.

#### Supabase Client Usage
Encourages typed Supabase queries with proper error handling.

#### Environment Variable Access
Ensures environment variables are properly validated and have fallbacks.

#### Design System Component Usage
Promotes using design system components for consistent UI.

#### API Key Security
Flags potential security issues with API keys.

#### Commented Code
Identifies commented debug code that should be removed before committing.

#### React Query Hook Naming
Ensures React Query hooks follow the 'use' prefix convention.

### Supabase Rules (supabase-rules.json)

#### Supabase Query Type Safety
Encourages using typed Supabase queries with generics for better type safety.

#### Supabase Error Handling
Ensures proper error handling in Supabase queries.

#### Supabase RLS Policy Check
Reminds to set up Row Level Security policies for database operations.

#### Supabase Auth Session Check
Suggests better patterns for handling authentication sessions.

#### Supabase Realtime Subscription
Reminds to clean up realtime subscriptions to prevent memory leaks.

#### Supabase Storage URL Construction
Encourages consistent patterns for storage URL generation.

### Design System Rules (design-system-rules.json)

#### Design System Component Usage
Encourages using design system components instead of raw HTML elements.

#### Inline Styles
Discourages the use of inline styles in favor of design system components.

#### Hard-coded Colors
Encourages using design system color tokens instead of hard-coded values.

#### Hard-coded Font Sizes
Promotes using typography tokens for consistent text styling.

#### Hard-coded Spacing
Encourages using spacing tokens for consistent layout.

#### Responsive Design
Suggests using design system breakpoint utilities for responsive layouts.

#### Accessibility Rules
Ensures proper ARIA attributes and alt text for better accessibility.

## Customization

Feel free to modify the rules to better suit your project's specific needs. The rule files are well-documented and easy to customize.

## Contributing

If you have suggestions for additional rules or improvements to existing ones, please create an issue or pull request.