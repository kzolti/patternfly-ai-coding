# PatternFly AI Helpers

AI coding helpers for [PatternFly](https://www.patternfly.org/) development. This repository provides plugins, rules, and documentation to help AI tools (Claude Code, Cursor, Copilot, etc.) generate accurate, best-practice PatternFly applications.

## Quick Start

### Claude Code

```bash
# Add the marketplace
/plugin marketplace add patternfly/ai-helpers

# Install the PatternFly React plugin
/plugin install pf-react@ai-helpers
```

After installation, use the commands in any project:

```bash
/coding-standards    # PatternFly v6 React coding standards
/test-generator      # Generate unit tests following Testing Library best practices
```

See [plugins/pf-react/](plugins/pf-react/) for full documentation.

### Cursor

Copy the `.cursor/rules/` directory into your project to enable PatternFly best-practice enforcement.

### Other AI Tools

Copy the `docs/` directory into your project workspace. AI tools index local files for context, so having the documentation present locally ensures accurate PatternFly guidance.

## Repository Structure

```
ai-helpers/
├── plugins/              # Claude Code plugins
│   └── pf-react/         # PatternFly React coding standards & test generation
├── docs/                 # AI-friendly PatternFly documentation
│   ├── guidelines/       # Coding standards, styling, accessibility
│   ├── components/       # Component-specific patterns
│   ├── charts/           # Chart guidelines
│   └── chatbot/          # Chatbot patterns
├── .cursor/rules/        # Cursor IDE rules
├── .claude-plugin/       # Plugin marketplace configuration
└── .claude/              # Claude Code settings
```

## Documentation

The `docs/` directory contains comprehensive, AI-friendly PatternFly documentation. See [docs/README.md](docs/README.md) for the full table of contents.

### Using Documentation with AI Tools

AI tools only index files present in your local workspace. To get the full benefit:

1. Clone or copy this repository (or at least the `docs/` directory) into your project
2. Open your project in your AI coding tool
3. The tool will automatically reference the documentation for PatternFly guidance

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on adding plugins, commands, documentation, and Cursor rules.

## References

- [PatternFly.org](https://www.patternfly.org/)
- [PatternFly React GitHub](https://github.com/patternfly/patternfly-react)
- [PatternFly MCP Server](https://github.com/patternfly/patternfly-mcp)

## License

[MIT](LICENSE)
