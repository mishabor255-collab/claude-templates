# DONE — add Todoist tasks from Claude

Todoist MCP connects Claude to your task list.
You need a Todoist account; this connection can read and change tasks.

## Connect in the app
1. In Claude Desktop, open Settings → Connectors.
2. Choose Add custom connector and name it Todoist.
3. Enter this server address: https://ai.todoist.net/mcp
4. Complete the Todoist sign-in flow and review permissions.
5. If unavailable, check account or workplace restrictions.
6. Start a new Claude chat and enable Todoist among its tools.

## Add your first task
7. Ask: “Add a task to collect my package tomorrow. First show the exact date and destination project, and wait for confirmation.”
8. Check the date, time zone, and project before confirming.
9. Open Todoist and verify that exactly one task was created.
10. Ask: “Show tomorrow’s tasks without changing anything.”

## Useful limits
A task’s due date does not automatically mean a notification is configured.
Check reminders separately in Todoist; availability depends on your plan and settings.
If a request fails, inspect the task list before retrying.
Revoke access through Todoist Settings → Integrations when needed.
Source: [todoist/todoist-mcp, Claude Desktop setup](https://github.com/todoist/todoist-mcp#claude-desktop).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
