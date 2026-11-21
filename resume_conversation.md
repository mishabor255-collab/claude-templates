# RESUME — pick up a Claude Code conversation

For Claude Code in the terminal. You need a previously saved conversation.
1. Open your terminal in the same project folder you used before.
2. Run:
```sh
claude --continue
```
The short form is `claude -c`.
3. Check that this is the conversation you wanted, then continue your task.

## Need a different conversation?
Run `claude --resume` in your terminal and choose from the list.
Already inside Claude Code? Enter `/resume` in its prompt instead.
Do not run `/resume` as a shell command.

## Conversation not found?
Check your project folder and whether saved history exists on this computer.
Without a matching session, `--continue` reports that no conversation was found.
This resumes a conversation; it does not restore deleted project files.
Check the current files before continuing: they may have changed.

[Official command reference](https://code.claude.com/docs/en/cli-reference).
[Official guide to resuming](https://code.claude.com/docs/en/common-workflows#resume-previous-conversations).
Not official Anthropic/OpenAI material.
