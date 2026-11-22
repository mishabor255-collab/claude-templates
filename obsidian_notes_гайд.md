# Obsidian MCP: работа в Claude Desktop

Нужен Claude Desktop на компьютере; эта локальная настройка не подключает Claude в браузере.
Предварительно: Obsidian и установленный uv/uvx: https://docs.astral.sh/uv/getting-started/installation/
Если среды запуска нет, сначала настрой её по инструкции разработчика; одного ZIP репозитория недостаточно.

1. В Obsidian открой Settings → Community plugins → Browse, установи и включи Local REST API. В настройках плагина возьми ключ и HTTPS-порт.
2. Открой меню приложения Claude → Settings → Developer → Edit Config.
3. Сохрани копию открытого файла. Добавь запись ниже внутрь существующего mcpServers, сохранив остальные записи.
Для пустой конфигурации подходит весь блок; для непустой объединяй записи, не создавай второй mcpServers.
```json
{"mcpServers": {"mcp-obsidian": {"command": "uvx", "args": ["mcp-obsidian"], "env": {"OBSIDIAN_API_KEY": "YOUR_LOCAL_KEY", "OBSIDIAN_HOST": "127.0.0.1", "OBSIDIAN_PORT": "27124"}}}}
```
4. В конфигурации замени YOUR_LOCAL_KEY и порт на свои значения. Ключ вводи только локально; держи Obsidian открытым.
5. Сохрани файл и полностью перезапусти Claude Desktop. При первом запуске потребуется интернет для загрузки пакета.
6. В новом чате проверь наличие подключённого инструмента. Если npx/uvx не найден, укажи полный путь к установленному приложению запуска.
7. Отправь запрос:
> Найди в Obsidian заметки со словами хлеб и бизнес. Покажи выдержки и пути исходных заметок. Ничего не меняй.
8. Разрешай только нужные чтения. Возможности MCP шире этого примера; не одобряй незапрошенные изменения.
9. Открой найденные источники и сравни результат с ними.

Репозиторий: https://github.com/MarkusPfundstein/mcp-obsidian
Настройка приложения: https://modelcontextprotocol.io/docs/develop/connect-local-servers

Плагин: https://github.com/coddingtonbear/obsidian-local-rest-api
Больше разборов: https://t.me/neuromentorrr
Не является официальным материалом Anthropic/OpenAI.
