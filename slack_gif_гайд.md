# ГУСЬ — сделать анимацию для чата в Claude

slack-gif-creator из anthropics/skills помогает создавать GIF для Slack.
Звёзды в ролике относятся ко всему репозиторию, а не одному навыку.

## Подготовь архив
1. Открой [репозиторий](https://github.com/anthropics/skills), выбери Code → Download ZIP.
2. Распакуй архив через Finder или Проводник.
3. Найди папку skills/slack-gif-creator и прочитай SKILL.md.
4. Сохрани все файлы этой папки, включая вспомогательный код.
5. Сожми именно папку slack-gif-creator в ZIP штатным меню файлового менеджера.

## В приложении Claude
6. В Settings → Capabilities включи Create and edit files, ранее Code execution and file creation.
7. Открой Customize → Skills → + → + Create skill → Upload a skill.
8. Загрузи ZIP с одной папкой навыка и включи навык.
9. Начни чат: «Используй slack-gif-creator. Сделай простого рисованного гуся: прыжок, поклон, плавный повтор. Без текста и логотипов. Нужен скачиваемый GIF для сообщения в Slack».
10. Если нужны библиотеки, попроси Claude подготовить их в среде создания файлов.

## Проверь результат
Скачай GIF, открой и проверь плавность повторения и размер файла.
Попроси уменьшить размер, если файл не подходит для твоего способа загрузки в Slack.
Навык не содержит готовую библиотеку персонажей и не отправляет GIF в Slack сам.
Если загрузку навыков запретила организация, потребуется помощь её администратора.
Источники: [инструкция навыка](https://github.com/anthropics/skills/blob/main/skills/slack-gif-creator/SKILL.md), [Skills в Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).
Больше разборов: https://t.me/neuromentorrr
Не является официальным материалом Anthropic/OpenAI.
