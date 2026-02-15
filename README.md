# claude-plugins

Personal Claude Code plugin marketplace for MCP servers.

## Plugins

| Plugin | Description |
|--------|-------------|
| `nvim-markdown-notes-memgraph` | Memgraph-powered knowledge graph MCP server for markdown notes |

## Usage

### Add the marketplace

```bash
# Local
/plugin marketplace add /home/rick/code/personal/claude-plugins

# From GitHub (once published)
/plugin marketplace add xpcoffee/claude-plugins
```

### Install a plugin

```bash
/plugin install nvim-markdown-notes-memgraph@claude-plugins
```

### Verify

```bash
claude mcp list
```

## Prerequisites

For `nvim-markdown-notes-memgraph`:

1. Install the package: `pip install nvim-markdown-notes-memgraph`
2. Start the backing services: `nvim-markdown-notes-memgraph start` (requires Docker)
3. The MCP server connects to Memgraph on `localhost:7687` and reads notes from `~/notes`
