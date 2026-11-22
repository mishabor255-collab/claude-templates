# Desktop Commander: use it in Claude Desktop

Use the installed Claude Desktop app; this local setup does not connect the browser version.
Prerequisite: Node.js LTS from https://nodejs.org/ using its standard installer.
If the runtime is missing, follow its installation instructions first; downloading the repository ZIP is not enough.

1. Start with a separate folder containing certificate copies. Supply its absolute path.
2. Open the Claude application menu → Settings → Developer → Edit Config.
3. Back up the file. Merge the entry below into its existing mcpServers object, preserving other entries.
Use the full block only for an empty configuration; do not add a second mcpServers object.
```json
{"mcpServers": {"desktop-commander": {"command": "npx", "args": ["-y", "@wonderwhy-er/desktop-commander"]}}}
```
4. Open the suggested documents yourself. Similar filenames do not imply identical contents.
5. Save and fully restart Claude Desktop. The first launch needs internet access to download the package.
6. Check that the tool is connected in a new chat. If npx/uvx cannot be found, use its installed absolute path.
7. Send this prompt:
> Find certificates in /absolute/path/to/copies. List paths, names and dates. Do not change files.
8. Approve only the reads needed here. The MCP has broader capabilities; decline unrequested changes.
9. Open the original sources and compare them with the result.

Repository: https://github.com/wonderwhy-er/DesktopCommanderMCP
App setup: https://modelcontextprotocol.io/docs/develop/connect-local-servers
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
