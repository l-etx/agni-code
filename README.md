# agni-code

> A curated Claude Code configuration — agents, skills, commands, and rules for production-ready development workflows.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-1.0.0-green.svg)](VERSION)

---

## What is agni-code?

**agni-code** is a focused, opinionated Claude Code plugin built on top of the [Everything Claude Code](https://github.com/affaan-m/everything-claude-code) project. It ships a curated subset of agents, skills, commands, and rules tuned for the workflows I actually use day-to-day.

---

## Contents

### Agents (25)

Specialized subagents for delegation via `claude --agent`:

| Agent | Purpose |
|---|---|
| `planner` | Implementation planning and task decomposition |
| `architect` | High-level system design |
| `code-architect` | Code-level architectural decisions |
| `a11y-architect` | Accessibility-first design |
| `code-reviewer` | General code quality review |
| `python-reviewer` | Python-specific review |
| `cpp-reviewer` | C++ review |
| `fastapi-reviewer` | FastAPI/REST API review |
| `database-reviewer` | Database schema and query review |
| `security-reviewer` | Security audit |
| `mle-reviewer` | Machine learning engineering review |
| `tdd-guide` | Test-driven development guidance |
| `code-explorer` | Codebase exploration and understanding |
| `code-simplifier` | Complexity reduction |
| `comment-analyzer` | Comment quality analysis |
| `doc-updater` | Documentation maintenance |
| `docs-lookup` | Documentation search and retrieval |
| `refactor-cleaner` | Safe refactoring |
| `performance-optimizer` | Performance analysis and optimization |
| `silent-failure-hunter` | Find silent errors and hidden bugs |
| `pr-test-analyzer` | Pull request test coverage analysis |
| `loop-operator` | Long-running agent loop management |
| `network-architect` | Network design |
| `network-config-reviewer` | Network configuration review |
| `network-troubleshooter` | Network diagnostics |

### Skills (34)

Workflow definitions loaded via `/skill`:

**Development**
- `tdd-workflow` — Test-driven development cycle
- `coding-standards` — Project coding standards enforcement
- `python-patterns` — Python idiomatic patterns
- `python-testing` — Python test writing
- `pytorch-patterns` — PyTorch/ML patterns
- `cpp-testing` — C++ testing patterns
- `mysql-patterns` — MySQL query patterns
- `mcp-server-patterns` — MCP server development

**Frontend & UI**
- `frontend-patterns` — Frontend architecture patterns
- `frontend-slides` — Slide deck generation
- `liquid-glass-design` — Liquid glass UI effects
- `ui-demo` — UI demo creation
- `ui-to-vue` — Convert UI designs to Vue

**Security**
- `security-review` — Code security review workflow
- `security-scan` — Automated security scanning
- `security-bounty-hunter` — Bug bounty hunting methodology

**Research & Analysis**
- `search-first` — Research-before-coding discipline
- `scientific-thinking-scholar-evaluation` — Academic paper evaluation
- `scientific-thinking-literature-review` — Systematic literature review
- `repo-scan` — Repository analysis
- `regex-vs-llm-structured-text` — When to use regex vs LLM
- `market-research` — Market and competitor analysis
- `product-capability` — Product capability mapping

**Network**
- `network-interface-health` — Interface health checks
- `network-config-validation` — Config validation
- `network-bgp-diagnostics` — BGP diagnostics

**Agents & Automation**
- `agentic-os` — Agentic operating system patterns
- `hookify-rules` — Hook configuration rules
- `data-scraper-agent` — Data scraping agent patterns
- `documentation-lookup` — Documentation search

**Writing & Productivity**
- `article-writing` — Technical article writing
- `strategic-compact` — Strategic planning compacts
- `token-budget-advisor` — Token budget management
- `click-path-audit` — UX click path analysis

### Commands (19)

Slash commands invoked directly in Claude Code:

| Command | Description |
|---|---|
| `/plan` | Create an implementation plan |
| `/plan-prd` | Generate a PRD and hand off to `/plan` |
| `/python-review` | Python code review |
| `/code-review` | General code review |
| `/security-scan` | Run security scan |
| `/refactor-clean` | Refactoring workflow |
| `/cpp-review` | C++ code review |
| `/cpp-build` | C++ build fix workflow |
| `/cpp-test` | C++ test workflow |
| `/fastapi-review` | FastAPI review |
| `/pr` | Pull request workflow |
| `/review-pr` | Review a pull request |
| `/update-docs` | Update documentation |
| `/loop-start` | Start an agent loop |
| `/loop-status` | Check loop status |
| `/hookify` | Configure hooks |
| `/hookify-configure` | Detailed hook configuration |
| `/hookify-help` | Hook help |
| `/hookify-list` | List configured hooks |

### Rules

Always-on guidelines applied to every session:

- `common` — Universal coding guardrails
- `python` — Python-specific rules
- `cpp` — C++ rules

---

## Installation

### Option A: Clone directly

```bash
git clone https://github.com/lteixeira93/agni-code.git ~/.claude/plugins/agni-code
```

### Option B: Install via script

```bash
curl -fsSL https://raw.githubusercontent.com/lteixeira93/agni-code/main/install.sh | bash
```

### Option C: Copy to project

Copy the relevant directories (`agents/`, `skills/`, `commands/`, `rules/`) into your project's `.claude/` folder.

---

## Usage

After installation, use agents via `claude --agent <name>` or invoke skills and commands directly in Claude Code:

```
/plan build a REST API with authentication
/python-review
/security-scan
```

---

## Credits

Built on top of [Everything Claude Code](https://github.com/affaan-m/everything-claude-code) by Affaan Mustafa — MIT licensed.

---

## License

MIT
