# KB MCP Server

MCP-сервер для управления базой знаний с полнотекстовым поиском.

## Установка

```bash
pip install -e .
```

## Быстрый старт

```bash
# Инициализация базы данных
python -m kb_mcp.cli init

# Создание проекта
python -m kb_mcp.cli project create "Мой проект" --desc "Описание"

# Добавление знаний
python -m kb_mcp.cli kb add <project_id> "Заголовок" "Контент" --tags api,docs

# Поиск
python -m kb_mcp.cli search "OAuth2"
```

## Архитектура

```
Проект → Требования → Знания
```

## MCP Tools

19 инструментов для работы с проектами, требованиями и знаниями.
