# PatternFly React Plugin

Claude Code plugin for PatternFly React development with coding standards enforcement and test generation.

## Installation

```bash
# Add the PatternFly marketplace
/plugin marketplace add patternfly/ai-helpers

# Install the plugin
/plugin install pf-react@ai-helpers
```

## Commands

### `/coding-standards`

Get guidance on PatternFly React best practices:

```
/coding-standards
> How should I structure a data table with filtering?
> Review this Table implementation for PatternFly v6 compliance
> What's the best component for displaying notifications?
```

### `/test-generator`

Generate comprehensive unit tests:

```
/test-generator
> Generate tests for my UserProfile component
> Create tests for this data fetching hook
```

## What's Included

### PatternFly MCP Server Integration

Both agents automatically connect to the [PatternFly MCP server](https://github.com/patternfly/patternfly-mcp) which provides:

- **`searchPatternFlyDocs`** - Search for component documentation
- **`usePatternFlyDocs`** - Get full docs and JSON schemas

This means agents have access to up-to-date PatternFly documentation without any manual configuration.

### Coding Standards Agent

Based on official PatternFly guidelines:

- Component composition patterns
- PatternFly v6 styling standards
- Design token usage
- Accessibility requirements (WCAG 2.1 Level AA)
- React and TypeScript best practices

### Test Generator Agent

Based on Testing Library best practices:

- User behavior testing over implementation details
- Semantic query strategies
- Proper mocking patterns
- Accessibility testing
- PatternFly-specific patterns

## File Structure

```
pf-react/
├── .claude-plugin/
│   └── plugin.json      # Plugin metadata + MCP server config
├── agents/
│   ├── coding-standards.md
│   └── test-generator.md
├── commands/
│   ├── coding-standards.md
│   └── test-generator.md
└── README.md
```

## Troubleshooting

**Commands not recognized:**
```bash
/plugin list                              # Verify plugin is installed
/plugin install pf-react@ai-helpers  # Reinstall if needed
```

**MCP server not connecting:**
```bash
/mcp status  # Check MCP server status
```

If MCP is unavailable, agents fall back to their built-in documentation.

## Sources

- [PatternFly.org](https://www.patternfly.org/)
- [PatternFly React GitHub](https://github.com/patternfly/patternfly-react)
- [PatternFly MCP Server](https://github.com/patternfly/patternfly-mcp)
- [React Testing Library](https://testing-library.com/docs/react-testing-library/intro)

## License

MIT
