# MCP — Model Context Protocol

This directory contains [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) server configuration files. MCP servers extend AI assistant capabilities by exposing tools (e.g. database queries, file system access) directly to the model.

## Configurations

| File | Description |
|------|-------------|
| [PostgreSqL_Connect.json](./PostgreSqL_Connect.json) | MCP server config for connecting to a PostgreSQL database |

## Usage

To use an MCP server configuration:

1. Open the file and set the `POSTGRES_CONNECTION_STRING` environment variable (or replace the placeholder value) with your actual connection string.
2. Reference the config file in your AI tool's MCP settings (e.g. VS Code Copilot, Claude Desktop).
3. The MCP server will expose database tools (`query`, `listDatabases`, etc.) to the model session.

> **Security**: Never commit real credentials. The `POSTGRES_CONNECTION_STRING` in `PostgreSqL_Connect.json` contains a placeholder value (`******localhost:5432/dbname`). Set it via an environment variable or a local `.env` file that is excluded from version control.

## Adding New MCP Configs

Create a new JSON file following the same structure as `PostgreSqL_Connect.json`. Each config should define:

```json
{
  "mcpServers": {
    "<server-name>": {
      "description": "...",
      "command": "npx",
      "args": ["-y", "<mcp-package>"],
      "env": { "<ENV_VAR>": "<placeholder>" }
    }
  }
}
```
