# AI Automation Overview

This document provides a high-level overview of the AI automation system — its purpose, architecture, and how the components fit together.

## Purpose

The AI automation framework enables orchestrated, guided AI agent execution with proper governance, quality assurance, and memory management. It provides a structured way to break complex projects into discrete, agent-executed steps that produce verifiable outputs.

## Key Components

### Agents
Agents are the workers of the system. Each agent is specialized for a particular domain (data, API, frontend, testing, etc.) and follows a defined lifecycle: receive inputs → execute → produce structured outputs → hand off to the next agent. See [`agents/agent-registry.md`](./agents/agent-registry.md).

### Skills
Skills are reusable, modular capabilities that agents can invoke. A skill encapsulates a specific task (e.g., "generate a SQL migration", "build a React component") and can be shared across multiple agents. See [`skills/skill-registry.md`](./skills/skill-registry.md).

### Workflows
Workflows orchestrate agents into multi-step processes. The numbered lifecycle workflows (WF-00 through WF-10) cover the full project lifecycle from intake to launch. See [`workflows/workflow-registry.md`](./workflows/workflow-registry.md).

### Prompts
Prompts initialize agents and provide stack-specific context. Each agent has a `prompt.md`; domain prompts (e.g., `api-prompt.md`) provide targeted guidance for a specific layer. See [`prompts/prompt-registry.md`](./prompts/prompt-registry.md).

### Governance
Governance documents define the rules agents must follow:
- [`ai-governance.md`](./ai-governance.md) — decision authority, audit, access control
- [`ai-security-rules.md`](./ai-security-rules.md) — data security, agent security, compliance
- [`ai-quality-checklist.md`](./ai-quality-checklist.md) — pre- and post-deployment quality gates

### Memory & Logs
Memory files persist decisions and learnings across sessions. Log files record every agent run and workflow execution. Both start empty and accumulate at runtime. See [`memory/`](./memory/) and [`logs/`](./logs/).

## How It All Connects

```
User prompt / task
    ↓
orchestrator-agent (reads agent-registry, workflow-registry)
    ↓
Appropriate workflow (WF-00 → WF-10)
    ↓
Specialized agents invoke skills → produce outputs → docs/agent-outputs/
    ↓
memory/ and logs/ updated
```

## Getting Started

1. Review the [Roadmap](./ai-automation-roadmap.md) to understand the project phases
2. Read [Governance](./ai-governance.md) for rules and access control
3. Follow [Security Rules](./ai-security-rules.md) before handling data
4. Use the [Quality Checklist](./ai-quality-checklist.md) before deploying
5. See [INDEX.md](./INDEX.md) for a full directory listing

