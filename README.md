h1 Graphic weather analitic
============================

## weather-prognosis

Получает прогноз погоды на ближайшие 5 дней по часам с [сайта погоды](http://api.openweathermap.org), приводит словарь с данными в строковый формат, загружает в файл `'json_dictionery'`

Получает на вход аргументы:

    dir /--app_id(id с сайта),
    dir /--city(необязательный, по дефолту Moscow)

Получает словарь с данными о погоде на каждый час в ближайшие 5 суток, выводит в файл.
Пример:

    dir /Users...\python.exe weather-prognosis.py --city London --app_id 7...0
***
## weather-analisys

Загружает словарь из из `'json_dictionery'` в виде строки, парсит его с помощью json.loads; Выводит график зависимости температуры от времени.

![Alt text](https://github.com/BikeevArtur/Phrase-Generator/blob/master/Figure_0.png?raw=true "Optional Title")

Затем (после закрытия окна с графиком) выводит круговую гистограмму с типами погоды: "пасмурно", "дождь"... в процентном соотношении.
