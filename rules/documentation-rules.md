Документация Websource формируется на основании следующих правил:

- rules/source-of-truth.md
- rules/audience.md
- registry/statuses.md
- registry/documentation-types.md
- registry/default-documentation-values.md

Для PHP-классов использовать:
- templates/php-class.md

Для JavaScript-модулей использовать:
- templates/js-module.md

Если тип документации не определён, сначала определить его через registry/documentation-types.md.

Если данные не подтверждены кодом, реестрами или существующей документацией, они не должны попадать в документацию.

Перед формированием frontmatter обязательно применять правила из:

registry/default-documentation-values.md

Если поле не должно выводиться согласно этому реестру, оно не должно присутствовать в итоговом Markdown.