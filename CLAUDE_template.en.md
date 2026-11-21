# CLAUDE.md — a rules template for Claude Code

<!--
How to use:
1. Copy this file into the root of your project (next to your src folder or README.md) and rename it to CLAUDE.md.
2. Replace the text in [square brackets] with your own. Delete anything you don't need.
3. Run `claude` in the project folder — it reads this file automatically.
You can edit it any time: the rules apply on the next start.
Note: these instructions guide Claude; they do not enforce access restrictions.
-->

## How to talk to me
- Explain things in plain English, no jargon. If a term is needed, explain it in one sentence.
- Before making changes, briefly describe the plan: what you'll change and in which files.
- After the work, give a short report: what was done, which files changed, whether it was tested.
- If you're unsure or the task is unclear, ask first — don't guess.

## About the project
- What it is: [e.g. a Telegram bot for booking appointments]
- Language and tools: [e.g. Python 3.12, aiogram]
- How to run it: [e.g. `python3 bot.py`]
- How to check it works: [e.g. `pytest`, or "open the bot and send /start"]

## What matters
- [e.g. all user-facing text in English]
- [e.g. file names in lowercase with underscores]

## Don't touch
- Never delete anything without my explicit OK.
- Don't edit files with passwords and keys (`.env`) and never print their contents.
- [e.g. the `data/` folder — it has real customer data]

## How to work with code
- Change only what I asked for; if you spot another problem, tell me first.
- Small steps: check after each change.
- Before big changes, suggest a git commit so we can roll back.
