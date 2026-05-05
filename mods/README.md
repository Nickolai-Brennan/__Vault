# AI Automation Framework

This directory contains the complete AI automation framework, including agents, skills, prompts, workflows, and supporting infrastructure.

## Structure

- **agents/**: Agent definitions and configurations
- **automations/**: Automated task definitions
- **commands/**: Slash commands and CLI command definitions
- **evals/**: Evaluation frameworks and results
- **instructions/**: Global instructions and coding standards
- **logs/**: Run logs and audit trails (append-only; start empty)
- **MCP/**: Model Context Protocol server configurations
- **memory/**: Project memory and decision logs (append-only; start empty)
- **prompts/**: Prompt templates and definitions
- **references/**: Reference documentation and guides
- **schemas/**: JSON schemas for validation
- **scripts/**: Utility and generation scripts
- **skills/**: Reusable skill modules
- **tasks/**: Task tracking and management
- **templates/**: Reusable templates
- **workflows/**: Workflow orchestration files

## Quick Links

- [AI Automation Overview](./AI_AUTOMATION_OVERVIEW.md)
- [Roadmap](./ai-automation-roadmap.md)
- [Governance](./ai-governance.md)
- [Security Rules](./ai-security-rules.md)
- [Quality Checklist](./ai-quality-checklist.md)

## File Generation Order

When bootstrapping a new project from this framework, generate files in this order:

```
1. instructions/
2. .github/copilot-instructions.md
3. .github/agents/
4. agents/
5. skills/
6. workflows/
7. prompts/
8. templates/
9. evals/
10. scripts/
11. commands/
12. docs/
13. frontend/
14. backend/
15. database/
16. api/
17. tests/
```
