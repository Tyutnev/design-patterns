# Единая точка доступа

План урока
1. Понятие
2. Описание
3. Пример

### 1)Понятие
**Единая точка доступа** - обеспечивает унифицированный интерфейс для интерфейсов в подсистеме. Front Controller определяет высокоуровневй интерфейс, упрощающий использование подсистемы.

### 2)Описание
В сложных веб-сайтах есть много одинаковых действий, которые надо производить во время обработки запросов. Это, например, контроль безопасности, многоязычность и настройка интерфейса пользователя. Когда поведение входного контроллера разбросано между несколькими объектами, дублируется большое количество кода. Помимо прочего возникают сложности смены поведения в реальном времени.

Паттерн Front Controller объединяет всю обработку запросов, пропуская запросы через единственный объект-обработчик. Этот объект содержит общую логику поведения, которая может быть изменена в реальном времени при помощи декораторов. После обработки запроса контроллер обращается к конкретному объекту для отработки конкретного поведения.

### 3)Пример
Реализация роутинга для поиска контроллера и действия в MVC приложениях