# Agent Registry

## Overview

All agents in this registry follow the standard four-file structure:
- `AGENT.md` — canonical definition, capabilities, I/O, operating instructions
- `prompt.md` — system prompt used to initialize the agent
- `rules.md` — domain rules, error handling, safety constraints, Do/Don't checklist
- `workflows.md` — workflow participation, integration points, handoff protocol

Output from each agent is saved to `docs/agent-outputs/<agent-name>/` and formatted using the shared YAML output template (see any `AGENT.md`).

---

## Core Agents

| Agent | Directory | Role |
|---|---|---|
| Orchestrator Agent | `orchestrator-agent/` | Entry point for all workflows; routes work, manages handoffs, synthesizes status |
| Project Planner Agent | `project-planner-agent/` | Converts requirements into project brief, roadmap, milestones, risk register |

## Data Agents

| Agent | Directory | Role |
|---|---|---|
| Data Cleanup Agent | `data-cleanup-agent/` | Cleans, normalizes, deduplicates, and validates raw datasets |
| Data Analysis Agent | `data-analysis-agent/` | Analyzes datasets; extracts insights, statistics, and patterns |

## Development Agents

| Agent | Directory | Role |
|---|---|---|
| Model Development Agent | `model-development-agent/` | Designs scoring/ML model specs, feature engineering, evaluation plans |
| Stats Visualization Agent | `stats-visualization-agent/` | Designs chart specs, dashboard layouts, visualization recommendations |

## Infrastructure Agents

| Agent | Directory | Role |
|---|---|---|
| API Agent | `api-agent/` | Designs REST/GraphQL contracts, OpenAPI specs, service boundaries |
| Frontend Dashboard Agent | `frontend-dashboard-agent/` | Designs UI component plans, page layouts, state management |
| Backend Agent | `backend-agent/` | Designs service architecture, business logic, data access patterns |
| Database Agent | `database-agent/` | Designs DB schemas, DDL SQL, ERDs, indexes, migration strategies |

## Support Agents

| Agent | Directory | Role |
|---|---|---|
| Documentation Agent | `documentation-agent/` | Generates READMEs, API refs, runbooks, architecture docs |
| Testing Agent | `testing-agent/` | Plans test strategy, test cases, coverage targets, QA checklists |
| Marketing Agent | `marketing-agent/` | Plans marketing strategy, messaging, content calendar, campaigns |
| Repo Maintenance Agent | `repo-maintenance-agent/` | Maintains repo health, changelogs, CI/CD hygiene |

---

## Additional Subdirectory Agents

These agents have full subdirectory structures but serve more specialised roles:

| Agent | Directory | Role |
|---|---|---|
| API Architect | `api-architect/` | Guides API design interactively; generates working connectivity code from developer-supplied specs |
| Mentor | `mentor/` | Mentor mode — challenges engineers' assumptions and guides problem-solving without writing code |

---

## Specialist Persona Agents

These agents use a single `.agent.md` file (YAML frontmatter + instructions) rather than the four-file structure. They are designed to be activated as Copilot personas or chat modes.

| Agent file | Name | Role |
|---|---|---|
| `arch.agent.md` | Senior Cloud Architect | Architecture design patterns, NFR requirements, diagrams |
| `devops-expert.agent.md` | DevOps Expert | Full DevOps infinity loop: Plan → Code → Build → Test → Release → Deploy → Operate → Monitor |
| `expert-nextjs-developer.agent.md` | Next.js Expert | Next.js 16 App Router, Server Components, Turbopack, TypeScript |
| `expert-react-frontend-engineer.agent.md` | Expert React Frontend Engineer | React 19.2 hooks, Server Components, Actions, TypeScript, performance |
| `go-mcp-expert.agent.md` | Go MCP Server Development Expert | Building MCP servers in Go using the official SDK |
| `markdown-accessibility-assistant.agent.md` | Markdown Accessibility Assistant | Improves markdown accessibility per GitHub best practices |
| `postgresql-dba.agent.md` | PostgreSQL Database Administrator | PostgreSQL administration, schema, and query work via the PostgreSQL extension |
| `prompt-builder.agent.md` | Prompt Builder | Expert prompt engineering and validation |
| `search-ai-optimization-expert.agent.md` | Search & AI Optimization Expert | SEO, AEO, and GEO with AI-ready content strategies |
| `task-planner.agent.md` | Task Planner | Creates actionable implementation plans with tracking files |
| `task-researcher.agent.md` | Task Researcher | Comprehensive project and codebase analysis before planning |
| `technical-content-evaluator.agent.md` | Technical Content Evaluator | Evaluates technical training materials for accuracy and pedagogy |
| `vision-reverse-breakdown.md` | Vision Reverse Breakdown | Reverse-engineers a finished product vision into systems, tasks, and MVP scope |

---

## Typical Workflow Sequence

```
orchestrator-agent
  → project-planner-agent   (WF-00)
  → data-cleanup-agent      (WF-02)
  → data-analysis-agent     (WF-03)
  → model-development-agent (WF-04)  [if ML needed]
  → database-agent          (WF-07)
  → api-agent               (WF-06)
  → backend-agent           (WF-06)
  → stats-visualization-agent (WF-05)
  → frontend-dashboard-agent  (WF-05)
  → testing-agent           (WF-08)
  → documentation-agent     (WF-09)
  → repo-maintenance-agent  (WF-10)
  → marketing-agent         (WF-10)
  → orchestrator-agent      (sign-off)
```

Agents may run in parallel when there are no dependencies between them. See individual `workflows.md` files for exact integration points.
