# ТЕКСТ — подключаем MarkItDown к приложению Claude

MarkItDown от Microsoft превращает PDF, Word, PowerPoint и Excel в простой текст (Markdown).
Claude получает текст без лишнего оформления — часто это компактнее, чем исходный файл.
Насколько меньше — зависит от файла. Сканы (картинки) без распознавания текста не помогут.

## Что нужно
- Приложение Claude Desktop (Mac или Windows).
- Python 3.10 или новее.

## Шаги
1. Один раз поставь сервер MarkItDown — в Терминале (Mac) или PowerShell (Windows):
   ```bash
   pip install markitdown-mcp
   ```
2. Узнай полный путь к программе: `which markitdown-mcp` (Mac) или `where markitdown-mcp` (Windows).
3. В Claude Desktop: **Настройки → Developer → Edit Config**. Откроется файл `claude_desktop_config.json`.
4. Добавь (вместо пути — свой из шага 2):
   ```json
   {
     "mcpServers": {
       "markitdown": { "command": "/полный/путь/к/markitdown-mcp" }
     }
   }
   ```
   Если в файле уже есть `mcpServers`, добавь только строку `"markitdown": {...}` внутрь.
5. Полностью закрой и снова открой Claude.
6. В чате попроси: «Конвертируй file:///Users/имя/Documents/учебник.pdf в Markdown и найди формулу дисперсии».

## Если не работает
- Проверь путь из шага 2 и запятые в JSON.
- В README есть вариант через Docker — он рекомендован для Claude Desktop.

Источник: https://github.com/microsoft/markitdown/tree/main/packages/markitdown-mcp
Больше разборов: https://t.me/neuromentorrr
Не является официальным материалом Anthropic или Microsoft.
