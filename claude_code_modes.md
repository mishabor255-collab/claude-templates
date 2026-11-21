# Cheat sheet: three Claude Code modes to get started

In the Claude Code terminal, press **Shift+Tab** to cycle modes:
**Manual → accept edits → plan**. The current mode is shown at the bottom of the window.

| Mode | Bottom of the screen | What Claude does | When to use |
|---|---|---|---|
| **Manual** | `manual mode on` | Asks before most edits and commands; pre-approved actions run without prompting | By default, while learning or on important projects |
| **Accept edits** | `accept edits on` | Automatically approves edits and some simple filesystem commands; other commands follow permission rules | When you trust the task and don't want to approve every edit |
| **Plan** | `plan mode on` | Explores the project and prepares a plan **without editing your code**; moves to edits only after you approve | Big tasks, unfamiliar projects, "make it pretty" |

## How to use plan mode
1. Press **Shift+Tab** until you see `plan mode on`.
2. Describe the task in plain words.
3. Read the plan. Want changes? Tell Claude what to adjust ("only the button, leave the rest alone").
4. Happy with it? Approve the plan and choose how edits are approved. Claude gets to work.

## Small but useful
- **Esc** interrupts the current action; completed changes remain.
- Use **Shift+Tab** to switch modes outside approval dialogs (inside the plan approval dialog it does something else).
- Put persistent project instructions into **CLAUDE.md** in your project folder (template next to this file).

There are more modes — see the official docs: <https://code.claude.com/docs/en/permission-modes>
Not an official Anthropic resource.
