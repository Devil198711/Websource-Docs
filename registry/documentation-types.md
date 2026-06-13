# Типы документации Websource

Этот файл описывает типы сущностей, которые могут документироваться в Websource.

## Подтверждённые типы

| Тип | Назначение | Пример пути документации |
|---|---|---|
| `classes` | PHP-классы ядра, админки, модулей и темы | `ru/api/classes/{slug}/latest.md` |
| `methods` | Методы PHP- и JS-классов | Внутри страницы класса или отдельным подразделом |
| `modules` | Модули ядра, админки или frontend-части | `ru/api/modules/{slug}/latest.md` |
| `functions` | Глобальные PHP-функции | `ru/api/functions/{slug}/latest.md` |
| `constants` | Глобальные PHP-константы | `ru/api/constants/{slug}/latest.md` |
| `globals` | Глобальные переменные окружения CMS | `ru/api/globals/{slug}/latest.md` |
| `options` | Настройки CMS и значения из таблицы `options` | `ru/api/options/{slug}/latest.md` |
| `routing` | Маршрутизация и типы страниц | `ru/api/routing/{slug}/latest.md` |
| `templates` | Шаблоны темы и подключаемые файлы темы | `ru/api/templates/{slug}/latest.md` |
| `ajax` | AJAX- и submit-обработчики | `ru/api/ajax/{slug}/latest.md` |
| `js-modules` | JavaScript-модули админки и frontend-части | `ru/api/js-modules/{slug}/latest.md` |
| `js-classes` | JavaScript-классы | `ru/api/js-classes/{slug}/latest.md` |
| `dom-actions` | DOM-события, data-атрибуты и actions | `ru/api/dom-actions/{slug}/latest.md` |
| `database` | Таблицы, схемы БД и методы работы со структурой БД | `ru/api/database/{slug}/latest.md` |
| `localization` | Языковые домены и локализация | `ru/api/localization/{slug}/latest.md` |

## Неподтверждённые типы

Эти типы пока не нужно добавлять в основную структуру документации, пока они не подтверждены кодом:

| Тип | Причина |
|---|---|
| `interfaces` | PHP-интерфейсы в прочитанных файлах не найдены |
| `traits` | PHP-трейты в прочитанных файлах не найдены |
| `hooks` | Отдельная система hook API пока не подтверждена |

## Правило добавления новых типов

Новый тип документации можно добавить только если:

1. он подтверждён кодом;
2. для него есть понятная структура файлов;
3. понятно, чем он отличается от уже существующих типов;
4. для него можно сделать отдельный шаблон или раздел в существующем шаблоне.

Если тип не подтверждён, его нельзя добавлять в публичную структуру документации как готовый раздел.