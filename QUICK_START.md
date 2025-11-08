# Quick Start Guide

## Installation (5 minutes)

### Step 1: Add the Marketplace

In Claude Code, run:

```bash
/plugin marketplace add heysarver/claude-code-lbildzinkas-marketplace
```

### Step 2: Install the Plugin

```bash
/plugin install fullstack-dev-suite@lbildzinkas-marketplace
```

### Step 3: Verify Installation

```bash
/help
```

You should see the custom commands and agents now available.

## Test Drive

### Try the Commit Command

```bash
/commit
```

This intelligent command will:
- Run pre-commit checks (lint, build, type check)
- Analyze your changes
- Create a conventional commit message
- Suggest splitting if multiple changes detected

### Use an Agent

Try asking:

```
"Create a FastAPI endpoint for user login with JWT authentication"
```

Claude will automatically:
- Use the `backend-security-coder` agent
- Apply FastAPI best practices from CLAUDE.md
- Include proper validation and error handling

### Backend Example

```
"Build a PostgreSQL database schema for an e-commerce platform"
```

Agents used: `database-optimizer`, `backend-architect`

### Frontend Example

```
"Create a responsive navbar with dark mode toggle using Tailwind"
```

Agents used: `frontend-developer`, `ui-ux-designer`

### Full Stack Example

```
"Implement a real-time notification system with WebSockets"
```

Agents used: `backend-architect`, `frontend-developer`, `performance-engineer`

## What's Different?

### Before Plugin

```
User: "Create an API endpoint"
Claude: Creates basic endpoint
```

### After Plugin

```
User: "Create an API endpoint"
Claude:
- Uses FastAPI conventions from CLAUDE.md
- Applies backend-security-coder agent
- Includes type hints, Pydantic models
- Adds error handling with guard clauses
- Uses async/await patterns
- Follows RORO pattern
```

## Next Steps

1. Read the [full README](./README.md) for detailed documentation
2. Explore the [plugin documentation](./plugins/fullstack-dev-suite/README.md)
3. Check out all 82+ agents in the `agents/` directory
4. Customize `CLAUDE.md` for your specific needs

## Troubleshooting

### Plugin Not Found

Make sure you added the marketplace first:
```bash
/plugin marketplace add heysarver/claude-code-lbildzinkas-marketplace
```

### Commands Not Available

Restart Claude Code after installation.

### Want to Update?

```bash
/plugin update fullstack-dev-suite@lbildzinkas-marketplace
```

## Support

- [GitHub Issues](https://github.com/heysarver/claude-code-lbildzinkas-marketplace/issues)
- [Claude Code Docs](https://docs.claude.com/en/docs/claude-code)

---

Happy coding with your new fullstack development superpowers!
