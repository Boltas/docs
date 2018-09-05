# Метод delete

Удаляет конфигурацию хостинга статических сайтов для корзины.


## Запрос {#request}

```
DELETE /{bucket}?website HTTP/1.1
```

### Path параметры {#path-parameters}

Параметр | Описание
----- | -----
`bucket` | Имя корзины.

### Query параметры {#parameters}

Параметр | Описание
----- | -----
`website` | Обязательный параметр для обозначения типа операции.

### Заголовки {#request-headers}

Используйте в запросе только [общие заголовки](../common-request-headers.md).


## Ответ {#response}

### Заголовки {#response-headers}

Ответ может содержать только [общие заголовки](../common-response-headers.md).

### Коды ответов {#response-codes}

Перечень возможных ответов смотрите в разделе [[!TITLE]](../response-codes.md).

Если конфигурация хостинга не существует, то [!KEYREF objstorage-name] ответит кодом 200.