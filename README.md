# DataOx Junior Python Developer Test #3 | Async Web Scraping www.kijiji.ca site #
Async Web Scraping www.kijiji.ca site with asyncio and save scraped information into PostgreSQL DB where ads id used as table id
***
### The project is built on libraries: ###
asyncio

aiohttp

BeautifulSoup

psycopg2


### Для запуска программы: ###
1. В файле database_async.py в строках 102-106 указать параметры подключения к БД PostgreSQL для создания БД проекта, пользователя и таблицы.
2. После этого запустить файл database_async.py. Будет создана БД, пользователь БД и таблица для записи данных.
3. Запустить файл async.py

Парсинг производиться асинхронно. На моем компьютере это занимает 2,5 минуты на 3200 записей. 

Отличие этой версии от https://github.com/akatendra/DataOx:
1. Парсинг производиться асинхронно с помощью asyncio и aiohttp.
2. Парсинг происходит быстрее в 10 раз: 2,5 минуты против 25 минут в первоначальном варианте.
3. Отказался от использования Selenium
4. Здесь в таблице, где хранятся данные парсинга в качестве уникального id используется id объявления на сайте.
5. Кода стало меньше.
6. Найдены и исправлены ошибки, которые не позволяли записать в БД некоторые объявления с сайта.

В файле requirements.txt - список установленных в venv библиотек.
***
