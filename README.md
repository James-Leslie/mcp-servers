# MCP Servers
A collection of local Python MCP (Model Context Protocol) servers for use with Cursor.

## Configuration
Clone the repo to a location of your choice, e.g. `~/mcp-servers`

Add any of the servers to Cursor by updating the MCP configuration as follows:

```json
{
    "mcpServers": {
        "<server-name>": {
            "command": "uvx",
            "args": [ 
                "~/mcp-servers/<server-name>/."
            ]
        }
    }
}
```

Place this in:
- `~/.cursor/mcp.json` for global access (cursor will have access from any project)
- `.cursor/mcp.json` for project-specific access
