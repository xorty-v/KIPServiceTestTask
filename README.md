# Тестовое задание на backend программиста

Реализовать асинхронную обработку запросов на .net core, тип приложения WebApi.
1. Метод для запроса пользовательской статистики POST /report/user_statistics. В тело
запроса передаем идентификатор пользователя, период с и по. Результат выполнения метода
- Guid запроса.
2. Метод получения информации о запросе GET /report/info. Параметр метода - Guid запроса.
Ответ - json в котором указан Guid запроса, процент выполнения запроса, и результат
выполнения, если он есть.

Приложение должно обрабатывать запрос не быстрее чем за X миллисекунд (вынести в
конфигурационный файл, по умолчанию установить 60 секунд), и рассчитывать процент
обработки в зависимости от пройденного времени с момента создания запроса.

Желательно использовать ORM, структуру базы данных делать через миграции.
Покрытие тестами будет большим плюсом.
