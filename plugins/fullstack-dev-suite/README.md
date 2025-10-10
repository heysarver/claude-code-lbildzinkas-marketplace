# Fullstack Development Suite Plugin

A comprehensive Claude Code plugin that provides development conventions, 82+ specialized AI agents, and custom workflows for professional fullstack development.

## Overview

This plugin transforms Claude Code into a powerful fullstack development environment with pre-configured best practices for:
- **Backend**: Python, FastAPI, uv package management, Pydantic v2
- **Frontend**: React, Vite, TypeScript, Tailwind CSS, Next UI, three.js

## Features

### 🎯 Development Conventions (CLAUDE.md)

Automatically injected coding standards and best practices that guide Claude's code generation:

#### Backend Standards
- Functional, declarative programming patterns
- Type hints and Pydantic models for validation
- Error-first handling with early returns and guard clauses
- Async/await patterns for I/O operations
- Performance optimization strategies
- FastAPI-specific patterns and middleware

#### Frontend Standards
- Functional React components with TypeScript
- Modern React 19+ patterns and hooks
- Tailwind CSS and Next UI integration
- Error boundaries and proper error handling
- Performance optimization with lazy loading
- Accessibility best practices

### 🤖 82+ Specialized AI Agents

Expert agents that are automatically invoked when relevant to your task:

#### Backend Development
- **backend-architect**: Design APIs, microservices, database schemas
- **backend-security-coder**: Secure coding, authentication, API security
- **fastapi-pro**: FastAPI development and async optimization
- **python-pro**: Modern Python 3.12+ with async patterns
- **django-pro**: Django 5.x with async views and DRF

#### Frontend Development
- **frontend-developer**: React 19, Next.js 15, modern architecture
- **typescript-pro**: Advanced TypeScript patterns and type safety
- **javascript-pro**: Modern JavaScript ES6+ and async patterns
- **ui-ux-designer**: Interface design, accessibility, design systems
- **flutter-expert**: Flutter development with Dart 3

#### Cloud & Infrastructure
- **cloud-architect**: AWS/Azure/GCP multi-cloud architecture
- **kubernetes-architect**: K8s, GitOps, service mesh, ArgoCD/Flux
- **terraform-specialist**: Advanced IaC, state management
- **deployment-engineer**: CI/CD pipelines, GitOps workflows
- **hybrid-cloud-architect**: Complex multi-cloud solutions

#### DevOps & Operations
- **devops-troubleshooter**: Incident response, debugging, observability
- **incident-responder**: SRE practices, incident management
- **performance-engineer**: Observability, optimization, Core Web Vitals

#### Database & Data
- **database-optimizer**: Query optimization, performance tuning
- **database-admin**: Cloud databases, automation, HA/DR
- **sql-pro**: Modern SQL, cloud-native databases
- **data-engineer**: Data pipelines, data warehouses, Spark
- **data-scientist**: Analytics, ML modeling, statistical analysis

#### Security
- **security-auditor**: DevSecOps, compliance, vulnerability assessment
- **frontend-security-coder**: XSS prevention, client-side security
- **backend-security-coder**: Input validation, authentication
- **mobile-security-coder**: Mobile-specific security patterns

#### AI & Machine Learning
- **ai-engineer**: LLM applications, RAG systems, AI agents
- **ml-engineer**: Production ML, model serving, A/B testing
- **mlops-engineer**: ML pipelines, experiment tracking, MLflow

#### Code Quality & Testing
- **code-reviewer**: AI-powered code analysis, security, performance
- **test-automator**: Modern test frameworks, self-healing tests
- **tdd-orchestrator**: Test-driven development discipline
- **debugger**: Debugging specialist for errors and failures

#### Specialized Development
- **blockchain-developer**: Smart contracts, DeFi, Web3
- **mobile-developer**: React Native, Flutter, native apps
- **unity-developer**: Unity games, C# scripts, URP/HDRP
- **golang-pro**: Go 1.21+ with modern patterns
- **rust-pro**: Rust 1.75+ with async and systems programming
- **java-pro**: Java 21+ with virtual threads
- **scala-pro**: Enterprise Scala with Akka/Pekko
- **elixir-pro**: Elixir with OTP and Phoenix LiveView
- **php-pro**: Modern PHP with generators and SPL
- **ruby-pro**: Ruby and Rails patterns
- **c-pro**: Efficient C with memory management
- **cpp-pro**: Modern C++ with RAII and smart pointers
- **csharp-pro**: C# with records and async/await

#### Architecture & Design
- **architect-review**: System design, clean architecture, DDD
- **graphql-architect**: GraphQL federation, performance
- **api-documenter**: OpenAPI 3.1, interactive docs
- **prompt-engineer**: Advanced prompting techniques

#### Documentation & Content
- **docs-architect**: Technical documentation from codebases
- **tutorial-engineer**: Step-by-step tutorials
- **reference-builder**: API documentation and references
- **mermaid-expert**: Diagrams for flowcharts, sequences, ERDs

#### SEO & Marketing
- **seo-content-writer**: SEO-optimized content creation
- **seo-content-planner**: Content outlines and topic clusters
- **content-marketer**: Content marketing strategies
- **seo-keyword-strategist**: Keyword analysis and optimization
- Plus many more SEO specialists...

#### Business & Finance
- **business-analyst**: Business intelligence, KPIs
- **quant-analyst**: Financial models, trading strategies
- **risk-manager**: Portfolio risk, hedging strategies

#### Other Specialists
- **payment-integration**: Stripe, PayPal integration
- **legal-advisor**: Privacy policies, terms of service
- **hr-pro**: HR policies, hiring, performance management
- **sales-automator**: Cold emails, proposals
- **customer-support**: AI-powered support systems
- **search-specialist**: Advanced search and research
- **error-detective**: Log analysis and error tracking
- **dx-optimizer**: Developer experience improvements
- **legacy-modernizer**: Refactoring and migrations
- **context-manager**: AI context engineering

### ⚡ Custom Slash Commands

#### /commit
Intelligent commit workflow with automatic checks:

**Features:**
- Automatic pre-commit checks (lint, build, type checking)
- Conventional commit format with emoji
- Smart commit splitting for multiple logical changes
- Git best practices enforcement

**Usage:**
```bash
# Standard commit with checks
/commit

# Skip pre-commit verification
/commit --no-verify
```

**What it does:**
1. Runs quality checks (unless --no-verify):
   - `pnpm lint` - Frontend code quality
   - `pnpm build` - Build verification
   - `ruff` - Backend code quality
   - `pyright` - Type safety
2. Checks staged files
3. Auto-stages if no files staged
4. Analyzes changes for splitting
5. Creates conventional commit messages

**Commit Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `perf`: Performance improvements
- `test`: Adding/fixing tests
- `chore`: Build process, tools, etc.

#### /run
Task execution helper for common development workflows.

#### /set-spec-file
Specification file management for project requirements.

## Installation

### From Marketplace

1. Add the marketplace:
```bash
/plugin marketplace add lbildzinkas/claude-code-market-place
```

2. Install the plugin:
```bash
/plugin install fullstack-dev-suite@lbildzinkas-marketplace
```

### Manual Installation

1. Clone the marketplace repository
2. Copy the `plugins/fullstack-dev-suite` directory to your local Claude plugins directory
3. Restart Claude Code

## Usage

### Automatic Features

Once installed, the plugin automatically:
- Injects development conventions into Claude's context
- Makes all 82+ agents available for proactive use
- Enables custom slash commands
- Applies coding standards to all generated code

### Example Workflows

#### Backend Development
```
"Create a FastAPI endpoint for user authentication with JWT tokens"
```
Claude will automatically:
- Use FastAPI best practices from CLAUDE.md
- Apply backend-security-coder agent for security
- Follow functional programming patterns
- Include proper error handling and validation

#### Frontend Development
```
"Build a responsive dashboard with React and Tailwind"
```
Claude will automatically:
- Use React/TypeScript conventions
- Apply frontend-developer agent
- Follow Next UI patterns
- Include accessibility features

#### Full Stack Feature
```
"Implement a real-time chat feature with WebSockets"
```
Claude will:
- Use multiple agents (backend-architect, frontend-developer, performance-engineer)
- Apply both backend and frontend conventions
- Ensure security and performance best practices

#### Code Review
```
"Review this code for security vulnerabilities and performance issues"
```
Claude will invoke:
- code-reviewer agent for general analysis
- security-auditor for security review
- performance-engineer for optimization suggestions

#### DevOps Tasks
```
"Set up a CI/CD pipeline with GitHub Actions and deploy to AWS"
```
Claude will use:
- deployment-engineer for CI/CD setup
- cloud-architect for AWS infrastructure
- kubernetes-architect if containers are involved

## Configuration

### Customizing Conventions

You can customize the development conventions by editing `CLAUDE.md` in your local copy of the plugin.

### Selective Agent Usage

While agents are invoked automatically, you can request specific agents:
```
"Use the rust-pro agent to optimize this performance-critical code"
```

## File Structure

```
fullstack-dev-suite/
├── .claude-plugin/
│   └── plugin.json              # Plugin metadata
├── CLAUDE.md                     # Development conventions
├── README.md                     # This file
├── agents/                       # 82+ agent definitions
│   ├── ai-engineer.md
│   ├── backend-architect.md
│   ├── cloud-architect.md
│   ├── code-reviewer.md
│   ├── frontend-developer.md
│   ├── security-auditor.md
│   └── ... (and 76 more)
└── commands/                     # Custom slash commands
    └── task/
        ├── commit.md
        ├── run.md
        └── set-spec-file.md
```

## Development Principles

This plugin enforces:

### Backend (Python/FastAPI)
- ✅ Functional, declarative programming
- ✅ Type hints for all function signatures
- ✅ Pydantic models for validation
- ✅ Error-first handling with guard clauses
- ✅ Async/await for I/O operations
- ✅ Dependency injection
- ✅ Performance optimization

### Frontend (React/TypeScript)
- ✅ Functional components with hooks
- ✅ TypeScript with strict type safety
- ✅ Declarative JSX
- ✅ RORO pattern (Receive an Object, Return an Object)
- ✅ Error boundaries
- ✅ Accessibility standards
- ✅ Performance optimization

### General
- ✅ Concise, technical responses
- ✅ Iteration over duplication
- ✅ Descriptive variable names
- ✅ Clear file structure
- ✅ Comprehensive error handling

## Version History

### 1.0.0
- Initial release
- 82+ specialized AI agents
- FastAPI and React development conventions
- Custom commit workflow command
- Comprehensive documentation

## Contributing

This plugin is part of a personal marketplace. For suggestions or issues, please open an issue on the [marketplace repository](https://github.com/lbildzinkas/claude-code-market-place/issues).

## License

MIT License

## Support

- [GitHub Issues](https://github.com/lbildzinkas/claude-code-market-place/issues)
- [Claude Code Documentation](https://docs.claude.com/en/docs/claude-code)

---

Built with ❤️ for professional fullstack development
