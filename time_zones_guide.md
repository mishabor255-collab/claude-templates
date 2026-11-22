# Time MCP: use it in Claude Desktop

Use the installed Claude Desktop app; this local setup does not connect the browser version.
Prerequisite: An existing uv/uvx installation: https://docs.astral.sh/uv/getting-started/installation/
If the runtime is missing, follow its installation instructions first; downloading the repository ZIP is not enough.

1. Use exact IANA timezone names: Europe/Moscow and Asia/Tokyo, rather than ambiguous abbreviations.
2. Open the Claude application menu → Settings → Developer → Edit Config.
3. Back up the file. Merge the entry below into its existing mcpServers object, preserving other entries.
Use the full block only for an empty configuration; do not add a second mcpServers object.
```json
{"mcpServers": {"time": {"command": "uvx", "args": ["mcp-server-time"]}}}
```
4. This example checks the time now. For a future meeting, verify the specific date and daylight saving rules separately.
5. Save and fully restart Claude Desktop. The first launch needs internet access to download the package.
6. Check that the tool is connected in a new chat. If npx/uvx cannot be found, use its installed absolute path.
7. Send this prompt:
> Use Time MCP. Show the current date and time in Europe/Moscow and Asia/Tokyo side by side. Do not schedule anything.
8. Approve only the reads needed here. The MCP has broader capabilities; decline unrequested changes.
9. Open the original sources and compare them with the result.

Repository: https://github.com/modelcontextprotocol/servers
App setup: https://modelcontextprotocol.io/docs/develop/connect-local-servers

Time configuration: https://github.com/modelcontextprotocol/servers/tree/main/src/time
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
