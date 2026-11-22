# GOOSE — make an animated chat GIF in Claude

slack-gif-creator from anthropics/skills helps create GIFs for Slack.
The video’s stars belong to the full repository, not this individual skill.

## Prepare the archive
1. Open the [repository](https://github.com/anthropics/skills); choose Code → Download ZIP.
2. Extract the archive in Finder or File Explorer.
3. Find skills/slack-gif-creator and read SKILL.md.
4. Keep the entire folder, including its supporting code.
5. Compress just the slack-gif-creator folder into a ZIP using your file manager.

## In Claude
6. Enable Create and edit files in Settings → Capabilities, previously Code execution and file creation.
7. Open Customize → Skills → + → + Create skill → Upload a skill.
8. Upload the single-skill ZIP and enable the skill.
9. Start a chat: “Use slack-gif-creator. Make a simple illustrated goose hop, bow, and loop smoothly. No text or logos. Provide a downloadable GIF for a Slack message.”
10. If libraries are missing, ask Claude to prepare them in its file-creation environment.

## Check the result
Download the GIF and inspect the loop and file size.
Ask for a smaller file if it does not fit your intended Slack upload.
The skill does not include a ready-made character library or automatically post to Slack.
If your organization blocks skill uploads, ask its administrator for help.
Sources: [skill instructions](https://github.com/anthropics/skills/blob/main/skills/slack-gif-creator/SKILL.md), [Claude skills](https://support.claude.com/en/articles/12512180-use-skills-in-claude).
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
