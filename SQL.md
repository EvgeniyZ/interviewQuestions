SQL
* Что такое кластерный индекс? Может ли быть более 1 кластерного? Может ли не быть кластерного?
* Что такое некластерный индекс и как он устроен?
* Что такое покрывающий (covering) index? Зачем он нужен?
* Что такое оконные функции (window functions)?

window functions have access to grouped individual rows and can add some of the attributes from those rows into the result set - OVER(), PARTITION BY and aggregate functions (COUNT, MIN, MAX, AVG, SUM, etc.)

* Как будет работать запрос без WHERE если есть индекс? 

SELECT * FROM ORDER BY field? 

* Как будут работать джоины по id? Оптимизирует ли их СУБД?
* Занимался ли настройкой БД в продакшене? (Always ON, availability groups?)
* Что если в продакшене твоя бд это узкое место? Как масштабировать базу данных?
* Расскажи про свой опыт нагрузки, хайлоада?
* Расскажи как бы ты боролся с нагрузкой и write операциями?

PostgreSQL
* В чём разница между Postgresql от других субд?

MVCC (Multi-Version concurrency control), нет READ UNCOMMITED, VACCUUM, indexes (hash index, btree, инвертированные, геометрические и проч.)
