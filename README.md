# Luiz's Fullstack Development Marketplace

A curated collection of professional development plugins for Claude Code, focused on fullstack development with FastAPI, React, and modern web technologies.

## Available Plugins

### Fullstack Development Suite

A comprehensive plugin that provides development conventions, specialized AI agents, and custom workflows for fullstack development.

**Features:**
- 🎯 **Development Conventions**: Pre-configured best practices for FastAPI/Python backend and React/Vite/Tailwind frontend
- 🤖 **82+ Specialized Agents**: Expert AI agents for various development tasks including:
  - Backend: API development, security, database optimization
  - Frontend: React development, UI/UX, performance optimization
  - DevOps: CI/CD, deployment, cloud architecture
  - Specialized: AI engineering, blockchain, mobile development, and more
- ⚡ **Custom Slash Commands**: Productivity-enhancing commands for common workflows
- 📚 **Comprehensive Documentation**: Detailed guides and best practices

**Tech Stack Coverage:**
- **Backend**: Python, FastAPI, uv package management, Pydantic v2
- **Frontend**: React, Vite, TypeScript, Tailwind CSS, Next UI, three.js, React Three Fiber
- **Patterns**: Functional programming, RORO pattern, clean architecture, DDD

## Installation

### Quick Start

1. Add this marketplace to Claude Code:
```bash
/plugin marketplace add lbildzinkas/claude-code-market-place
```

2. Install the Fullstack Development Suite:
```bash
/plugin install fullstack-dev-suite@lbildzinkas-marketplace
```

3. Verify installation:
```bash
/help
```

You should now see the custom agents and commands available in your Claude Code environment.

## What's Included

### Development Guidelines (CLAUDE.md)

Comprehensive coding standards and best practices including:

#### Backend Guidelines
- Functional, declarative programming patterns
- Type hints and Pydantic models for validation
- Error handling with early returns and guard clauses
- Performance optimization strategies
- Async/await patterns for I/O operations

#### Frontend Guidelines
- Functional React components with TypeScript
- Modern React patterns and hooks
- Tailwind CSS and Next UI integration
- Error boundaries and proper error handling
- Performance optimization techniques

### Specialized Agents

The plugin includes 82+ expert agents across multiple domains:

**Backend & API Development**
- `backend-architect`: API design, microservices, database schemas
- `backend-security-coder`: Secure coding, authentication, API security
- `fastapi-pro`: FastAPI development and optimization
- `python-pro`: Modern Python 3.12+ development

**Frontend Development**
- `frontend-developer`: React 19, Next.js 15, modern architecture
- `typescript-pro`: Advanced TypeScript patterns
- `ui-ux-designer`: Interface design, accessibility, design systems

**Cloud & DevOps**
- `cloud-architect`: Multi-cloud infrastructure, IaC
- `kubernetes-architect`: K8s, GitOps, service mesh
- `deployment-engineer`: CI/CD pipelines, deployment automation
- `devops-troubleshooter`: Incident response, debugging

**Database & Performance**
- `database-optimizer`: Query optimization, performance tuning
- `database-admin`: Cloud databases, automation, reliability
- `performance-engineer`: Observability, optimization

**Security**
- `security-auditor`: DevSecOps, compliance, vulnerability assessment
- `frontend-security-coder`: XSS prevention, client-side security

**AI & Advanced Topics**
- `ai-engineer`: LLM applications, RAG systems, AI agents
- `ml-engineer`: Production ML, model serving
- `data-scientist`: Analytics, ML modeling, statistical analysis

**Code Quality**
- `code-reviewer`: Code analysis, security, performance
- `test-automator`: Test automation, quality engineering
- `tdd-orchestrator`: Test-driven development

And many more specialized agents for various development needs!

### Custom Commands

- `/commit`: Intelligent commit workflow with conventional commits
- `/run`: Task execution helpers
- `/set-spec-file`: Specification management

## Usage Examples

### Using Development Conventions

The plugin automatically injects development guidelines into Claude's context, ensuring consistent code generation:

```bash
# Claude will automatically follow FastAPI best practices
"Create a new API endpoint for user authentication"

# Frontend code will follow React/TypeScript conventions
"Build a responsive navigation component with Tailwind"
```

### Using Specialized Agents

Agents are automatically available and can be proactively invoked by Claude when relevant:

```bash
# Backend security review
"Review this authentication code for security vulnerabilities"
# → backend-security-coder agent will be used

# Frontend performance optimization
"Optimize the rendering performance of this React component"
# → frontend-developer or performance-engineer agent will be used

# Cloud architecture design
"Design a scalable AWS infrastructure for this application"
# → cloud-architect agent will be used
```

### Using Custom Commands

```bash
# Create a well-formatted commit with automatic checks
/commit

# Run with pre-commit verification disabled
/commit --no-verify
```

## Plugin Structure

```
plugins/fullstack-dev-suite/
├── .claude-plugin/
│   └── plugin.json          # Plugin metadata
├── CLAUDE.md                 # Development guidelines
├── agents/                   # 82+ specialized AI agents
│   ├── ai-engineer.md
│   ├── backend-architect.md
│   ├── cloud-architect.md
│   └── ... (and many more)
└── commands/                 # Custom slash commands
    └── task/
        ├── commit.md
        ├── run.md
        └── set-spec-file.md
```

## Contributing

This is a personal marketplace, but suggestions and feedback are welcome! Please open an issue if you have ideas for improvements.

## License

MIT License - See individual plugin licenses for details.

## Support

For issues or questions:
- Open an issue on [GitHub](https://github.com/lbildzinkas/claude-code-market-place/issues)
- Check the [Claude Code documentation](https://docs.claude.com/en/docs/claude-code)

## Version History

### 1.0.0 (Initial Release)
- Fullstack Development Suite plugin
- 82+ specialized AI agents
- Development conventions for FastAPI and React
- Custom commit workflow command
- Comprehensive documentation

---

Made with ❤️ for the Claude Code community
