# JProfiler MCP Server

[![ej-technologies/jprofiler-mcp MCP server](https://glama.ai/mcp/servers/ej-technologies/jprofiler-mcp/badges/score.svg)](https://glama.ai/mcp/servers/ej-technologies/jprofiler-mcp)

[JProfiler](https://www.ej-technologies.com/jprofiler) is a Java profiler with AI agent
integration via the [Model Context Protocol](https://modelcontextprotocol.io).
Profile CPU hotspots, memory allocations, JDBC queries, HTTP calls and more
directly from your AI coding assistant.

Listed on [Glama](https://glama.ai/mcp/servers/ej-technologies/jprofiler-mcp).

## Installation

### Claude Code

```
claude mcp add jprofiler -- npx -y @ej-technologies/jprofiler-mcp
```

### Cursor

Listed on [cursor.directory](https://cursor.directory/plugins/jprofiler).

[![Install MCP Server](https://cursor.com/deeplink/mcp-install-dark.svg)](https://cursor.directory/plugins/jprofiler)

### Codex

```
codex mcp add jprofiler -- npx -y @ej-technologies/jprofiler-mcp
```

### Gemini CLI

```
gemini mcp add jprofiler npx -y @ej-technologies/jprofiler-mcp@latest
```

### Other MCP clients

Use the following npx invocation as the MCP server command in your client's configuration:

```
npx -y @ej-technologies/jprofiler-mcp@latest
```

For clients that use a JSON configuration file (Claude Desktop, Windsurf, VS Code, etc.):

```json
{
  "mcpServers": {
    "jprofiler": {
      "command": "npx",
      "args": ["-y", "@ej-technologies/jprofiler-mcp"]
    }
  }
}
```

### Optional arguments

- `--filter <patterns>` — Comma-separated list of tool name patterns to include
- `--subsystems <list>` — Comma-separated list of subsystems to enable
- `--max-depth <n>` — Maximum call tree expansion depth

## License

JProfiler requires a license. On first use, you can start a free 10-day evaluation
or enter an existing license key. Purchase at https://www.ej-technologies.com/store/jprofiler.

License terms: https://www.ej-technologies.com/jprofiler/license
