# DataOx Junior Python Developer Test #3 | Async Web Scraping www.kijiji.ca site #
Async Web Scraping www.kijiji.ca site with asyncio and save scraped information into PostgreSQL DB where ads id used as table id
***
### The project is built on libraries: ###
asyncio

BeautifulSoup

psycopg2


### Для запуска программы: ###
1. В файле database_async.py в строках 102-106 указать параметры подключения к БД PostgreSQL для создания БД проекта, пользователя и таблицы.
2. После этого запустить файл database.py_async. Будет создана БД, пользователь БД и таблица для записи данных.
3. Запустить файл async.py

Парсинг производиться асинхронно. На моем компьютере это занимает 2,5 минуты на 3200 записей. 

Отличие этой версии в том, что здесь в таблице, где хранятся данные парсинга в качестве уникального id используется id объявления на сайте.

В файле requirements.txt - список установленных в venv библиотек.
***
