# TEXT — connect MarkItDown to the Claude app

Microsoft's MarkItDown turns PDF, Word, PowerPoint and Excel files into plain text (Markdown).
Claude gets clean text without extra formatting — often more compact than the original file.
How much you save depends on the file. Scans (images) won't help without text recognition.

## You need
- The Claude Desktop app (Mac or Windows).
- Python 3.10 or newer.

## Steps
1. Install the MarkItDown server once — in Terminal (Mac) or PowerShell (Windows):
   ```bash
   pip install markitdown-mcp
   ```
2. Find its full path: `which markitdown-mcp` (Mac) or `where markitdown-mcp` (Windows).
3. In Claude Desktop: **Settings → Developer → Edit Config**. This opens `claude_desktop_config.json`.
4. Add this (use your path from step 2):
   ```json
   {
     "mcpServers": {
       "markitdown": { "command": "/full/path/to/markitdown-mcp" }
     }
   }
   ```
   If the file already has `mcpServers`, just add the `"markitdown": {...}` line inside it.
5. Fully quit and reopen Claude.
6. Ask in chat: "Convert file:///Users/name/Documents/textbook.pdf to Markdown and find the variance formula".

## If it doesn't work
- Check the path from step 2 and the commas in the JSON.
- The README also has a Docker option, which is recommended for Claude Desktop.

Source: https://github.com/microsoft/markitdown/tree/main/packages/markitdown-mcp
More tips: https://t.me/neuromentor_en
Not an official Anthropic or Microsoft resource.
