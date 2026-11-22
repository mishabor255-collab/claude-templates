# Use invoice-organizer in Claude

A skill supplies reusable instructions. Use Claude on the web or Claude Desktop.
Skills and code execution availability depend on account and organization settings.

1. Open the repository: https://github.com/ComposioHQ/awesome-claude-skills
2. Choose Code → Download ZIP and extract it using Finder or File Explorer.
3. Locate invoice-organizer and read SKILL.md before uploading.
4. Compress just the invoice-organizer folder, including its contents, into a separate ZIP.
5. Enable Code execution and file creation in Settings → Capabilities; newer layouts call it Create and edit files.
6. Open Customize → Skills → “+” → Create skill → Upload a skill.
7. Upload your ZIP and enable the skill in the list.
8. Start a new chat with your source material; for receipts, upload copies rather than a local folder path.
9. Send this prompt:
> Use invoice-organizer on the uploaded receipt copies. Extract date, vendor, amount, currency and original filename. Flag gaps. Return a table and a ZIP of renamed copies; preserve originals.
10. Check dates, amounts and currencies against originals. This workflow does not determine tax deductibility.

If the skill is not used, name it explicitly in your prompt and check its toggle.
A skill alone does not grant access to your computer; this workflow uses uploaded material.
Skill instructions: https://github.com/ComposioHQ/awesome-claude-skills/blob/master/invoice-organizer/SKILL.md
Upload help: https://support.claude.com/en/articles/12512180-use-skills-in-claude
More tips: https://t.me/neuromentor_en
This is not official Anthropic/OpenAI material.
