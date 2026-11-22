# MAP — diagrams inside a Claude chat

Excalidraw MCP creates diagrams with editing inside compatible chat clients.
This guide uses its remote connector, without a local installation.

## App steps
1. In Claude, open **Customize → Connectors**.
2. Choose **Add → Custom → Web**.
3. Name it Excalidraw and use the README's address: `https://mcp.excalidraw.com`.
4. Click **Continue**, review the detected sign-in options, then finish with **Add**.
5. Older layouts use **Settings → Connectors → Add custom connector**.
6. In a new chat, allow Excalidraw tools and send the prompt below.
7. Open the diagram, check labels, and request layout changes in chat.

## Copy this prompt
“Draw this in Excalidraw: Organizer → Guests; Organizer → Venue; Venue → Catering. Use only these relationships. Ask about missing relationships. Do not add logos.”
For a family example, replace names with fictional ones and supply only necessary relationships.
Check every arrow's direction. A neat drawing is not proof of a correct diagram.

## Troubleshooting
Workplace accounts may require an administrator to add the connector.
Inline diagrams need MCP Apps support. Update the app or try Claude on the web.
This connects to an external server; leave out unnecessary personal details.
Sources: [README and server address](https://github.com/excalidraw/excalidraw-mcp), [Claude connector setup](https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
