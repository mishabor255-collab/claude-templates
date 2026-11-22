# SPIN — a chore wheel in Claude

An artifact opens beside the chat and can be a small interactive tool.
Open Claude on the web or Desktop.

## Steps
1. Check **Settings → Capabilities → Create and edit files**.
2. Older layouts call this **Code execution and file creation**.
3. Start a new chat and send the prompt below.
4. Open the resulting artifact beside your conversation.
5. Enter only people who actually participate in the chores.
6. Press the button and request fixes in the chat if anything fails.

## Copy this prompt
“Create an interactive chore-wheel artifact. Include a names field, a Spin button, and one selected participant. Give everyone an equal chance. Display the result prominently. No registration or external services.”
“Handle an empty list gracefully. Ignore blank lines rather than treating them as participants.”

## Check it
Try no names, one name, and several different names.
With one participant, that person must win; an empty list should show a helpful message.
A few spins cannot prove fairness. Ask Claude to explain the selection method.
This example does not require or promise storage between visits.
Workplace administrators may control access to file creation.
Source: [Artifacts features and settings](https://support.claude.com/en/articles/17153992-what-are-artifacts-and-how-do-i-use-them).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
