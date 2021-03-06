Для оформления сообщения коммита следует использовать следующий шаблон:

    <type>(<scope>): <subject>
    <BLANK LINE>
    <body>

## Заголовок

### Тип коммита

Возможные типы:
* feature - используется при добавлении новой функциональности уровня приложения
* fix - если исправили какую-то серьезную багу
* docs - всё, что касается документации
* style - исправляем опечатки, исправляем форматирование
* refactor - рефакторинг кода приложения
* test - всё, что связано с тестированием
* chore - обычное обслуживание кода

Можно указывать несколько типов через запятую.

### Область действия

Здесь следует написать затронутые части (например, `lynx` или `tool_chain`)

### Сообщение

**Лучше написать грамотно по-русски, чем неграмотно по-английски!**

Общий стиль:

    действие (с маленькой буквы) + для какой сущности + (необязательно подробности)

**На английском:**

    fix NoMethodError in RemoteReader

Первое слово - глагол в неопределнной форме.

**На русском:**

    исправление ошибки NoMethodError в RemoteReader'е

Первое слово - отглагольное существительное.

Не нужно писать в сообщении номер таска из Джиры или тикета с Гитхаба - для этого есть тело коммита (см. далее).

## Например:
    fix(lynx): fix NoMethodError in RemoteReader
    docs(all): provide README.md with "Commit messages" section
    style(csv): исправление форматирования в bin/csv2json

## Тело

Заполнение тела коммита опционально. Нужно в том случае, если описание решенной проблемы достаточно сложно и не может уместиться в строку заголовка. Также сюда можно писать номер закрываемого (закрываемых) тасков из Джиры или тикетов с Гитхаба. Тело сообщения отделяется от заголовка одной пустой строкой и заполняется произвольно.

## Например:
    fix(lynx): fix NoMethodError in RemoteReader

    Closes #65