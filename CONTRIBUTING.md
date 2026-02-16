# Contributing to PatternFly AI Helpers

We welcome contributions of new plugins, commands, agents, documentation, and Cursor rules.

## Repository Structure

```
plugins/          # Claude Code plugins (each with commands/, agents/, skills/)
docs/             # AI-friendly PatternFly documentation
.cursor/rules/    # Cursor IDE rules
.claude-plugin/   # Plugin marketplace configuration
```

## Adding a New Claude Code Plugin

1. Create a new directory under `plugins/your-plugin-name/`
2. Add a `.claude-plugin/plugin.json` with required metadata:
   ```json
   {
     "name": "your-plugin-name",
     "description": "What your plugin does",
     "version": "0.0.1",
     "author": {
       "name": "Your Name"
     }
   }
   ```
3. Add commands under `commands/` and/or agents under `agents/` as `.md` files
4. Register your plugin in `.claude-plugin/marketplace.json`
5. Add a `README.md` documenting your plugin's commands and usage

## Adding a Command or Agent to an Existing Plugin

1. Add your `.md` file to the appropriate `commands/` or `agents/` directory
2. Commands need frontmatter with at minimum a `description` field
3. Agents need frontmatter with `name`, `description`, and `color` fields
4. Do **not** hardcode a `model:` in agent frontmatter -- let users choose their preferred model

## Adding Documentation

1. Add markdown files under `docs/` following the existing directory structure
2. Update `docs/README.md` (table of contents) to link to your new content

## Adding Cursor Rules

1. Add `.mdc` files to `.cursor/rules/`
2. Follow the existing frontmatter pattern with `description`, `globs`, and `alwaysApply`

## Submitting Changes

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## Guidelines

- Use kebab-case for directory and file names
- Include clear descriptions in all frontmatter
- Test your plugins locally before submitting
- Keep documentation concise and AI-friendly
