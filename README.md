# Простенький многопоточный сервер и клиент.
Решение должно быть на С\С++ (С++ предпочтительнее) и кроссплатформенное, т.е. использовать **posix** функции. в случае С++ можно и нужно использовать **boost**, сторонние библиотеки не допускаются

Протокол поверх tcp\ip разработать самостоятельно

Функционал не очень важен. Например, это может быть групповой чат (просто текстовый, консольный)

Основные обязательные функции:
- гостевой вход
- авторизованный вход (без изысков, данные и права пользователей можно захаркодить, но пароли естественно в открытом виде не хранить)
- массовая рассылка сообщений всем подключенным клиентам
- с админского аккаунта должны быть доступны функции:
- листинг списка всех клиентов с их айпи-адресами (важный момент - нужна поддержка IPv6)
- "кик" выбранного клиента
- "бан"" клиента по айпи на заданное время (например, в секундах)
