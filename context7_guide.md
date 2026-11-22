# DOCS — current library documentation in Claude

Context7 retrieves library documentation. It does not automatically fix your website.
Use Claude on the web or Desktop with connector access.

## Connect without a terminal
1. Open the [Context7 directory listing](https://claude.ai/directory/37153cd7-b17c-470e-8b46-007e2859e0f3) (linked in the Context7 repository README).
2. Add the connector and complete any sign-in it requests.
3. Find it under **Customize → Connectors**, or **Settings → Connectors** in older layouts.
4. For manual setup, choose **Add → Custom → Web** and enter `https://mcp.context7.com/mcp`.
5. Follow the authentication form; enter an API key in connector settings if required, never in a chat.
6. Start a new chat and allow Context7 through the connectors menu.

## Try this prompt
“Use Context7. Here are my library, version, and error: [insert details]. Find matching documentation, link it, and suggest a minimal fix. Tell me if that version is unavailable.”
If you do not know the version, ask Claude to inspect your project's dependency file first.
Check that Context7 was actually called and that the linked documentation matches your library.
Test the proposed fix separately. Retrieved documentation is not a guarantee of correct code.

## If access fails
A workplace account may require administrator approval; Context7 has request limits.
If asked to sign in or upgrade, check the service terms instead of repeatedly retrying.
Sources: [repository and Add to Claude link](https://github.com/upstash/context7), [Claude connectors](https://support.claude.com/en/articles/11176164-use-connectors-to-extend-claude-s-capabilities).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
