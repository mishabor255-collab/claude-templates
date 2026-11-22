# invoice-organizer в приложении Claude

Навык — набор инструкций для Claude. Работай в веб-приложении или Claude Desktop.
Доступность Skills и выполнения кода зависит от настроек аккаунта и организации.

1. Открой репозиторий: https://github.com/ComposioHQ/awesome-claude-skills
2. Выбери Code → Download ZIP и распакуй архив через Finder или Проводник.
3. Найди папку invoice-organizer; прочитай SKILL.md перед загрузкой.
4. Сожми только папку invoice-organizer вместе с её содержимым в отдельный ZIP.
5. В Claude включи Code execution and file creation в Settings → Capabilities; в обновлённом интерфейсе — Create and edit files.
6. Открой Customize → Skills → «+» → Create skill → Upload a skill.
7. Загрузи подготовленный ZIP и включи навык в списке.
8. Начни новый чат и добавь свои исходные данные; для чеков загружай копии файлов, а не путь к папке на компьютере.
9. Отправь запрос:
> Используй invoice-organizer. Разбери загруженные копии чеков: дата, продавец, сумма, валюта, исходное имя. Не угадывай пропуски. Дай таблицу и ZIP с переименованными копиями, сохрани исходники.
10. Сверь даты, суммы и валюты с оригиналами; этот разбор не определяет налоговые вычеты.

Если навык не применяется, явно назови его в запросе и проверь переключатель Skills.
Навык сам по себе не открывает доступ ко всему диску; здесь используются загруженные данные.
Описание навыка: https://github.com/ComposioHQ/awesome-claude-skills/blob/master/invoice-organizer/SKILL.md
Справка по загрузке: https://support.claude.com/en/articles/12512180-use-skills-in-claude
Больше разборов: https://t.me/neuromentorrr
Не является официальным материалом Anthropic/OpenAI.
