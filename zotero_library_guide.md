# Zotero MCP: use it in Claude Desktop

Use the installed Claude Desktop app; this local setup does not connect the browser version.
Prerequisite: Zotero 7+ and an existing uv/uvx installation: https://docs.astral.sh/uv/getting-started/installation/
If the runtime is missing, follow its installation instructions first; downloading the repository ZIP is not enough.

1. In Zotero → Settings → Advanced, enable the local API and keep Zotero open. Add two papers and their available PDFs.
2. Open the Claude application menu → Settings → Developer → Edit Config.
3. Back up the file. Merge the entry below into its existing mcpServers object, preserving other entries.
Use the full block only for an empty configuration; do not add a second mcpServers object.
```json
{"mcpServers": {"zotero": {"command": "uvx", "args": ["zotero-mcp-server", "serve"], "env": {"ZOTERO_LOCAL": "true"}}}}
```
4. Verify quotes against the PDFs and compare article versions. Library search does not guarantee access to every attachment.
5. Save and fully restart Claude Desktop. The first launch needs internet access to download the package.
6. Check that the tool is connected in a new chat. If npx/uvx cannot be found, use its installed absolute path.
7. Send this prompt:
> Find these two titles in Zotero. Compare findings with quotes and page references. Say when full text is unavailable.
8. Approve only the reads needed here. The MCP has broader capabilities; decline unrequested changes.
9. Open the original sources and compare them with the result.

Repository: https://github.com/54yyyu/zotero-mcp
App setup: https://modelcontextprotocol.io/docs/develop/connect-local-servers

Zotero configuration: https://github.com/54yyyu/zotero-mcp/blob/main/server.json
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
