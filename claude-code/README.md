# PatternFly Claude Code Plugins

[Claude Code](https://docs.anthropic.com/en/docs/claude-code) plugins for PatternFly development.

## Available Plugins

### [pf-react](plugins/pf-react/)

Coding standards and test generation for PatternFly React applications.

**Commands:**
- `/coding-standards` - PatternFly v6 React coding standards
- `/test-generator` - Generate unit tests following Testing Library best practices

**Features:**
- Automatic integration with [PatternFly MCP server](https://github.com/patternfly/patternfly-mcp)
- Real-time access to PatternFly documentation and component schemas
- Based on official PatternFly guidelines

## Installation

```bash
# Add the PatternFly marketplace
/plugin marketplace add patternfly/patternfly-ai-coding

# Install the pf-react plugin
/plugin install pf-react@patternfly-ai-coding
```

## Usage

After installation, the commands work in any project:

```bash
cd ~/my-patternfly-project
claude

# Use the agents
/coding-standards
/test-generator
```

## Sources

- [PatternFly.org](https://www.patternfly.org/)
- [PatternFly React GitHub](https://github.com/patternfly/patternfly-react)
- [PatternFly MCP Server](https://github.com/patternfly/patternfly-mcp)
- [React Testing Library](https://testing-library.com/docs/react-testing-library/intro)
