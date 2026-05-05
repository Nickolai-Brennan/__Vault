# mods/ Directory Index

This index lists every subdirectory in `mods/` with its purpose and key files. File counts are approximate; run `scripts/validate_file_tree.py` to get current counts.

## Root Files

| File | Purpose |
|------|---------|
| [README.md](./README.md) | Framework overview, structure, and quick links |
| [AI_AUTOMATION_OVERVIEW.md](./AI_AUTOMATION_OVERVIEW.md) | High-level overview of the automation system |
| [ai-automation-roadmap.md](./ai-automation-roadmap.md) | Phased roadmap with milestones |
| [ai-governance.md](./ai-governance.md) | Governance policies and principles |
| [ai-quality-checklist.md](./ai-quality-checklist.md) | Pre- and post-deployment quality checklist |
| [ai-security-rules.md](./ai-security-rules.md) | Security rules for agents and data |

## Subdirectories

### [agents/](./agents/)
Agent definitions and configurations. Each production agent has a four-file structure (`AGENT.md`, `prompt.md`, `rules.md`, `workflows.md`). Specialist persona agents use a single `.agent.md` file.

Key files: `agent-registry.md`, `agent-template.md`

### [automations/](./automations/)
Automated task definitions and schedules.

Key files: `automation-registry.md`, `automation-template.md`

### [commands/](./commands/)
Slash commands and CLI command definitions for the automation framework.

Key files: `README.md`

### [evals/](./evals/)
Evaluation frameworks, eval templates, and results.

Key files: `eval-template.md`, `agent-evals.md`, `prompt-evals.md`, `workflow-evals.md`

### [instructions/](./instructions/)
Global instructions, domain rules, and coding standards for agents and developers.

Key files: `global-ai-instructions.md`, `copilot-instructions.md`, `coding-standards.md`, `security-rules.md`

### [logs/](./logs/)
Append-only run logs and audit trails. These files begin empty and accumulate entries over agent runs.

Key files: `agent-run-log.md`, `workflow-run-log.md`, `error-log.md`, `release-log.md`

### [MCP/](./MCP/)
Model Context Protocol (MCP) server configuration files.

Key files: `README.md`, `PostgreSqL_Connect.json`

### [memory/](./memory/)
Project memory, decision logs, and learnings. These files begin empty and accumulate entries over time.

Key files: `project-memory.md`, `decision-log.md`, `lessons-learned.md`

### [prompts/](./prompts/)
Prompt templates and prompt definitions for use with agents.

Key files: `prompt-registry.md`, `prompt-template.md`

### [references/](./references/)
Reference documentation and design guides.

Key files: `ai-agent-architecture.md`, `prompt-engineering-guide.md`, `workflow-design-guide.md`, `api-design-guide.md`

### [schemas/](./schemas/)
JSON schemas for validating agents, skills, prompts, workflows, and other artifacts.

Key files: `agent.schema.json`, `skill.schema.json`, `prompt.schema.json`, `workflow.schema.json`, `project.schema.json`

### [scripts/](./scripts/)
Utility Python scripts for generating, validating, and maintaining framework artifacts.

Key files: `generate_agent.py`, `generate_skill.py`, `validate_file_tree.py`, `validate_prompts.py`

### [skills/](./skills/)
Reusable skill modules. Each skill has a `SKILL.md` and optional `evals/`, `references/`, `scripts/`, and `templates/` subdirectories. Packaged skills are distributed as `.zip` files.

Key files: `skill-registry.md`, `SKILLS.md` (conceptual skill taxonomy), `skill-template/`

### [tasks/](./tasks/)
Task tracking and management files.

Key files: `task-schema.md`, `task-template.md`, `backlog.md`, `active-tasks.md`, `completed-tasks.md`

### [templates/](./templates/)
Reusable templates for creating new agents, skills, prompts, workflows, tasks, and projects.

Key files: `agent-template.md`, `skill-template.md`, `project-template.md`, `project-types/`

### [workflows/](./workflows/)
Workflow orchestration files. Numbered workflows (`00–10`) follow the standard lifecycle; additional workflows cover specific build and operational patterns.

Key files: `workflow-registry.md`, `workflow-template.md`, `00-project-intake.workflow.md` – `10-launch-review.workflow.md`

