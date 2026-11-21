# FILE — point Claude Code to a file with @

Use this in the Claude Code prompt, not in your shell.
1. Open Claude Code in your project folder.
2. Find the path to the existing file you want to discuss.
3. Put `@` directly before the path, with no space:
```text
Explain the login function in @src/login.js. Do not edit anything yet.
```
`src/login.js` is an example: replace it with your actual file path.
Relative paths start from your working folder; absolute paths work too.

## Why it helps
A mention identifies a specific file and adds its contents to context when they fit the limits.
Type `@` for path suggestions; check the selected path before sending.
Try a small text file first.
A directory mention such as `@src/` adds a file listing, not all the code.

## Check the result
Compare the filename and explanation with your actual code.
A file mention does not prevent Claude from accessing other files.
An exact path provides clearer context, but does not guarantee a correct answer.

[Official documentation](https://code.claude.com/docs/en/common-workflows).
Not official Anthropic/OpenAI material.
