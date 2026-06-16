# Конфигурация Jira для дизайн-команды MyLink

## Общее подключение

| Параметр | Значение |
|---|---|
| cloudId | `bf61b230-67a7-4150-82eb-4981e9ddfd51` |
| Сайт | `mycar-group.atlassian.net` |
| Тип задачи | `Задача` (Task) |
| Приоритеты | High / Medium / Low |

## Проекты

### MLDS — Design System
- **Ключ проекта:** `MLDS`
- **Доска:** https://mycar-group.atlassian.net/jira/software/c/projects/MLDS/boards/1660
- **Для чего:** работа с компонентами, токенами, паттернами дизайн-системы
- **Префикс названия:** `Design: ...`

### DML — Design MyLink
- **Ключ проекта:** `DML`
- **Доска:** https://mycar-group.atlassian.net/jira/software/projects/DML/boards/902
- **Для чего:** продуктовые задачи и исследования команды
- **Префикс для product:** `[Продукт] ...`
- **Префикс для board:** `Действие: ...` (Аудит, Бенчмарк, Ресерч и т.п.)
- **Обязательные поля:** `customfield_10626` = `{ "id": "10345" }` (Designer approve = Yes)

## Исполнители

| Имя | accountId | Контекст |
|---|---|---|
| Assema Muzapbarova | `712020:0c45ea9c-1cf6-4ac2-9f89-3f17d187493d` | Дефолт для /board (аудиты) |

*Добавляй новых членов команды по мере необходимости.*

## Лейблы

### По типу задачи
| Тип | Лейблы |
|---|---|
| Design System | `design-system`, `components` |
| Product | `ux`, `product` |
| Board — Аудит | `audit`, `design-qa` |
| Board — Бенчмарк | `benchmark`, `research` |
| Board — Ресерч | `research` |
| Board — Конкурентный обзор | `competitive`, `research` |

### Дополнительные
| Лейбл | Когда |
|---|---|
| `tech-debt` | Технический долг по дизайну |
| `copy` | UX-копирайтинг |
| `accessibility` | A11y проблемы |

## Приоритеты по умолчанию

| Тип | Приоритет |
|---|---|
| Design System | Medium |
| Product | По влиянию (уточняется) |
| Board (аудит, ресерч) | High |

### Когда какой приоритет
- **High** — блокирует пользователя, критичная UX-проблема, важный аудит
- **Medium** — улучшение опыта, работа с ДС, тех долг
- **Low** — мелкие визуальные правки, nice-to-have
