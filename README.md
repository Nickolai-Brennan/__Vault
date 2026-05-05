## Title
### Subtitle


```
system/
├── README.md
├── SYSTEM_OVERVIEW.md
├── roadmap.md
├── governance.md
├── security-rules.md
├── quality-checklist.md


boost-mods/
│   ├── README.md
│   ├── boost-mod-registry.md
│   ├── boost-mod-template.md
│   ├── daily-project-review.md
│   ├── weekly-roadmap-review.md
│   ├── data-refresh-check.md
│   ├── model-retraining-check.md
│   ├── dashboard-quality-check.md
│   ├── broken-link-check.md
│   ├── repo-cleanup-check.md
│   └── changelog-generator.md
│
├── agents/
│   ├── README.md
│   ├── agent-registry.md
│   ├── agent-template.md
│   ├── orchestrator-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── project-planner-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── data-cleanup-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── data-analysis-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── model-development-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── stats-visualization-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── api-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── frontend-dashboard-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── backend-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── database-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── documentation-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── testing-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   ├── marketing-agent/
│   │   ├── AGENT.md
│   │   ├── prompt.md
│   │   ├── rules.md
│   │   └── workflows.md
│   └── repo-maintenance-agent/
│       ├── AGENT.md
│       ├── prompt.md
│       ├── rules.md
│       └── workflows.md
│
├── skills/
│   ├── README.md
│   ├── skill-registry.md
│   ├── skill-template/
│   │   ├── SKILL.md
│   │   ├── assets/
│   │   ├── scripts/
│   │   ├── templates/
│   │   └── references/
│   ├── project-intake-skill/
│   │   └── SKILL.md
│   ├── data-cleaning-skill/
│   │   └── SKILL.md
│   ├── notebook-query-skill/
│   │   └── SKILL.md
│   ├── model-formula-skill/
│   │   └── SKILL.md
│   ├── dashboard-design-skill/
│   │   └── SKILL.md
│   ├── api-design-skill/
│   │   └── SKILL.md
│   ├── database-schema-skill/
│   │   └── SKILL.md
│   ├── markdown-docs-skill/
│   │   └── SKILL.md
│   ├── code-review-skill/
│   │   └── SKILL.md
│   └── launch-checklist-skill/
│       └── SKILL.md
│
├── prompts/
│   ├── README.md
│   ├── prompt-registry.md
│   ├── prompt-template.md
│   ├── project-startup.prompt.md
│   ├── roadmap-builder.prompt.md
│   ├── data-cleaning.prompt.md
│   ├── data-analysis.prompt.md
│   ├── model-builder.prompt.md
│   ├── equation-builder.prompt.md
│   ├── dashboard-ui.prompt.md
│   ├── api-builder.prompt.md
│   ├── database-builder.prompt.md
│   ├── documentation-builder.prompt.md
│   ├── testing-review.prompt.md
│   └── deployment-review.prompt.md
│
├── workflows/
│   ├── README.md
│   ├── workflow-registry.md
│   ├── workflow-template.md
│   ├── 00-project-intake.workflow.md
│   ├── 01-data-collection.workflow.md
│   ├── 02-data-cleanup.workflow.md
│   ├── 03-data-analysis.workflow.md
│   ├── 04-model-development.workflow.md
│   ├── 05-dashboard-build.workflow.md
│   ├── 06-api-build.workflow.md
│   ├── 07-database-build.workflow.md
│   ├── 08-testing-validation.workflow.md
│   ├── 09-documentation.workflow.md
│   └── 10-launch-review.workflow.md
│
├── instructions/
│   ├── README.md
│   ├── global-ai-instructions.md
│   ├── copilot-instructions.md
│   ├── coding-standards.md
│   ├── repo-rules.md
│   ├── docs-rules.md
│   ├── data-rules.md
│   ├── api-rules.md
│   ├── database-rules.md
│   ├── frontend-rules.md
│   ├── testing-rules.md
│   └── security-rules.md
│
├── plugins/
│   ├── README.md
│   ├── plugin-registry.md
│   ├── plugin-template/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── github-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── google-drive-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── slack-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── notion-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── airtable-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── postgres-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── stripe-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── email-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── calendar-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── browser-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── web-scraper-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── file-system-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── vector-db-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   ├── analytics-plugin/
│   │   ├── PLUGIN.md
│   │   ├── config.json
│   │   ├── manifest.json
│   │   ├── src/
│   │   ├── tests/
│   │   └── docs/
│   └── deployment-plugin/
│       ├── PLUGIN.md
│       ├── config.json
│       ├── manifest.json
│       ├── src/
│       ├── tests/
│       └── docs/
│
├── commands/
│   ├── README.md
│   ├── command-registry.md
│   ├── command-template.md
│   ├── slash-commands.md
│   ├── cli-commands.md
│   ├── agent-commands.md
│   ├── workflow-commands.md
│   ├── automation-commands.md
│   ├── repo-commands.md
│   ├── data-commands.md
│   ├── deployment-commands.md
│   └── commands/
│       ├── init-project.command.md
│       ├── create-agent.command.md
│       ├── create-skill.command.md
│       ├── create-workflow.command.md
│       ├── run-agent.command.md
│       ├── run-workflow.command.md
│       ├── validate-prompts.command.md
│       ├── validate-tree.command.md
│       ├── generate-docs.command.md
│       ├── clean-repo.command.md
│       ├── sync-memory.command.md
│       ├── refresh-data.command.md
│       ├── rebuild-index.command.md
│       ├── deploy-preview.command.md
│       └── launch-review.command.md
│
├── hooks/
│   ├── README.md
│   ├── hook-registry.md
│   ├── hook-template.md
│   ├── lifecycle-hooks.md
│   ├── git-hooks.md
│   ├── agent-hooks.md
│   ├── workflow-hooks.md
│   ├── automation-hooks.md
│   ├── security-hooks.md
│   └── hooks/
│       ├── pre-agent-run.hook.md
│       ├── post-agent-run.hook.md
│       ├── pre-workflow-run.hook.md
│       ├── post-workflow-run.hook.md
│       ├── pre-prompt-change.hook.md
│       ├── post-prompt-change.hook.md
│       ├── pre-commit.hook.md
│       ├── pre-push.hook.md
│       ├── post-merge.hook.md
│       ├── on-file-change.hook.md
│       ├── on-error.hook.md
│       ├── on-deploy.hook.md
│       ├── on-schedule.hook.md
│       ├── on-security-risk.hook.md
│       └── on-quality-fail.hook.md
│
├── config/
│   ├── README.md
│   ├── ai.config.json
│   ├── agents.config.json
│   ├── workflows.config.json
│   ├── plugins.config.json
│   ├── commands.config.json
│   ├── hooks.config.json
│   ├── boost-mods.config.json
│   ├── permissions.config.json
│   ├── environments.config.json
│   └── secrets.example.env
│
├── runtime/
│   ├── README.md
│   ├── runtime-state.json
│   ├── active-agents.json
│   ├── active-workflows.json
│   ├── plugin-state.json
│   ├── command-history.json
│   ├── hook-events.json
│   ├── boost-mod-events.json
│   └── queue-state.json
│
├── tasks/
│   ├── README.md
│   ├── task-schema.md
│   ├── task-template.md
│   ├── backlog.md
│   ├── active-tasks.md
│   ├── blocked-tasks.md
│   ├── completed-tasks.md
│   └── task-tags.md
│
├── memory/
│   ├── README.md
│   ├── project-memory.md
│   ├── decision-log.md
│   ├── assumptions-log.md
│   ├── lessons-learned.md
│   ├── reusable-patterns.md
│   └── agent-feedback-log.md
│
├── evals/
│   ├── README.md
│   ├── eval-template.md
│   ├── prompt-evals.md
│   ├── agent-evals.md
│   ├── workflow-evals.md
│   ├── code-quality-evals.md
│   ├── data-quality-evals.md
│   └── model-output-evals.md
│
├── scripts/
│   ├── README.md
│   ├── generate_agent.py
│   ├── generate_skill.py
│   ├── generate_prompt.py
│   ├── generate_workflow.py
│   ├── generate_task_list.py
│   ├── generate_boost_mod.py
│   ├── validate_file_tree.py
│   ├── validate_prompts.py
│   ├── update_changelog.py
│   └── repo_cleanup.py
│
├── schemas/
│   ├── README.md
│   ├── agent.schema.json
│   ├── skill.schema.json
│   ├── prompt.schema.json
│   ├── workflow.schema.json
│   ├── task.schema.json
│   ├── boost-mod.schema.json
│   ├── plugin.schema.json
│   ├── command.schema.json
│   ├── hook.schema.json
│   ├── eval.schema.json
│   └── memory.schema.json
│
├── templates/
│   ├── README.md
│   ├── agent-template.md
│   ├── skill-template.md
│   ├── prompt-template.md
│   ├── workflow-template.md
│   ├── task-template.md
│   ├── boost-mod-template.md
│   ├── plugin-template.md
│   ├── command-template.md
│   ├── hook-template.md
│   ├── eval-template.md
│   ├── report-template.md
│   └── changelog-template.md
│
├── references/
│   ├── README.md
│   ├── ai-agent-architecture.md
│   ├── prompt-engineering-guide.md
│   ├── workflow-design-guide.md
│   ├── data-pipeline-guide.md
│   ├── dashboard-design-guide.md
│   ├── api-design-guide.md
│   ├── database-design-guide.md
│   ├── plugin-design-guide.md
│   ├── command-design-guide.md
│   ├── hook-design-guide.md
│   └── automation-best-practices.md
│
└── logs/
    ├── README.md
    ├── agent-run-log.md
    ├── workflow-run-log.md
    ├── prompt-change-log.md
    ├── plugin-log.md
    ├── command-log.md
    ├── hook-log.md
    ├── boost-mod-log.md
    ├── error-log.md
    └── release-log.md
