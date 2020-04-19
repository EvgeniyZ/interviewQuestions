Паттерны проектирования
* SOLID
* KISS
* DRY
* YAGNI
* Что такое и чем отличаются пессимистичная и оптимистичная блокировки? Pessimistic Locking is when you lock the record     for your exclusive use until you have finished with it. Optimistic Locking is a strategy where you read a record, take      note of a version number (other methods to do this involve dates, timestamps or checksums/hashes) and check that the        version hasn't changed before you write the record back.
* CQRS, Event sourcing.

Microservices and scaling
* Что такое вертикальное масштабированние\горизонтальное масштабирование?
* Как собирать метрики микро-сервиса? Какие это метрики (CPU, Memory - потребление ресурсов) и бизнес-логика?
* Зачем собирать метрики на уровне контейнера, пода, кластера? Какие это метрики?
* Twelve-factor app, основные (Stateless, Transactional)
* Какими тулами для развёртывания приложения пользовался?
* Как организовать доставку и масштабирование приложения?
* Работал ли с шинами сообщений? (RabbitMQ, Kafka, Azure Service Bus)
* Как можно устроить версионирование для клиентов (HTTP based) или для шины сообщений?
