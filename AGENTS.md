# agni-code — Agent Instructions

This is a **curated Claude Code plugin** providing 25 specialized agents, 34 skills, 19 commands, and automated hook workflows for software development.

**Version:** 1.0.0

## Core Principles

1. **Agent-First** — Delegate to specialized agents for domain tasks
2. **Test-Driven** — Write tests before implementation, 80%+ coverage required
3. **Security-First** — Never compromise on security; validate all inputs
4. **Immutability** — Always create new objects, never mutate existing ones
5. **Plan Before Execute** — Plan complex features before writing code

## Available Agents

| Agent | Purpose | When to Use |
|-------|---------|-------------|
| planner | Implementation planning | Complex features, refactoring |
| architect | System design and scalability | Architectural decisions |
| code-architect | Code-level design decisions | Module/component design |
| a11y-architect | Accessibility design | UI with accessibility requirements |
| tdd-guide | Test-driven development | New features, bug fixes |
| code-reviewer | Code quality and maintainability | After writing/modifying code |
| python-reviewer | Python-specific review | Python projects |
| cpp-reviewer | C/C++ code review | C and C++ projects |
| fastapi-reviewer | FastAPI/REST API review | FastAPI endpoints |
| database-reviewer | Schema and query review | Database changes |
| security-reviewer | Vulnerability detection | Before commits, sensitive code |
| mle-reviewer | ML engineering review | ML/AI model code |
| code-explorer | Codebase navigation and understanding | Unfamiliar codebases |
| code-simplifier | Complexity reduction | Overengineered code |
| comment-analyzer | Comment quality | Documentation review |
| doc-updater | Documentation maintenance | Updating docs |
| docs-lookup | Documentation search | Finding references |
| refactor-cleaner | Safe refactoring | Code maintenance |
| performance-optimizer | Performance analysis | Bottleneck investigation |
| silent-failure-hunter | Find silent errors | Defensive code review |
| pr-test-analyzer | PR test coverage | Before merging |
| loop-operator | Agent loop management | Long-running workflows |
| network-architect | Network design | Infrastructure planning |
| network-config-reviewer | Network config review | Router/switch configs |
| network-troubleshooter | Network diagnostics | Connectivity issues |

## Delegation Rules

- Use **planner** before implementing any feature > 2 files
- Use **security-reviewer** before any commit touching auth, crypto, or user data
- Use **tdd-guide** when writing new features to ensure tests come first
- Use **code-reviewer** after significant changes
- Use **refactor-cleaner** when removing dead code
- Use **network-troubleshooter** for connectivity or latency investigations

## Key Skills

Invoke with the skill name in your prompt or via `/skill <name>`:

- `tdd-workflow` — TDD cycle
- `security-scan` — Security scanning
- `python-patterns` — Python best practices
- `search-first` — Research before coding
- `coding-standards` — Project standards

## Key Commands

- `/plan` — Implementation planning
- `/python-review` — Python review
- `/code-review` — General review
- `/security-scan` — Security scan
- `/cpp-review` — C++ review
- `/refactor-clean` — Refactoring
