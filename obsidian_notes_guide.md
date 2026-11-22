# Obsidian MCP: use it in Claude Desktop

Use the installed Claude Desktop app; this local setup does not connect the browser version.
Prerequisite: Obsidian and an existing uv/uvx installation: https://docs.astral.sh/uv/getting-started/installation/
If the runtime is missing, follow its installation instructions first; downloading the repository ZIP is not enough.

1. In Obsidian, open Settings → Community plugins → Browse; install and enable Local REST API. Find its API key and HTTPS port in plugin settings.
2. Open the Claude application menu → Settings → Developer → Edit Config.
3. Back up the file. Merge the entry below into its existing mcpServers object, preserving other entries.
Use the full block only for an empty configuration; do not add a second mcpServers object.
```json
{"mcpServers": {"mcp-obsidian": {"command": "uvx", "args": ["mcp-obsidian"], "env": {"OBSIDIAN_API_KEY": "YOUR_LOCAL_KEY", "OBSIDIAN_HOST": "127.0.0.1", "OBSIDIAN_PORT": "27124"}}}}
```
4. Replace YOUR_LOCAL_KEY and the port with your local values. Keep the key local and leave Obsidian open.
5. Save and fully restart Claude Desktop. The first launch needs internet access to download the package.
6. Check that the tool is connected in a new chat. If npx/uvx cannot be found, use its installed absolute path.
7. Send this prompt:
> Search Obsidian for bread and business. Show excerpts and original note paths. Change nothing.
8. Approve only the reads needed here. The MCP has broader capabilities; decline unrequested changes.
9. Open the original sources and compare them with the result.

Repository: https://github.com/MarkusPfundstein/mcp-obsidian
App setup: https://modelcontextprotocol.io/docs/develop/connect-local-servers

Plugin: https://github.com/coddingtonbear/obsidian-local-rest-api
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
