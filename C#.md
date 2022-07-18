* Из чего состоит платформа .NET? (CLR, BCL, Standard Libraries - System.*, Intermediate Language) .NET 5, .Net Core and .NET Standard
* Что такое Common Type System? (Value types and reference types)
* Как происходит дебаг приложения? (генерация и использование .pdb файлов)
* Что такое Serializable attribute, зачем он нужен? - передача объекта в файл, по сети (via SOAP или Binary) - BinaryFormatter, SoapFormatter
* Каким атрибутом можно скрыть поле класса чтобы оно не передавалось наружу клиентам? (NotMapped)
* Какие настройки есть у EF? Что такое ProxyCreationEnable? Что такое Proxy классы в EF? Object State Manager в EF?
* Когда возникает StackOverflowException и как его отловить, исправить, продебажить на продакшене?
* String это value или reference type? В чём отличие от других reference types (immutable)
* Интернирование строк - что такое, зачем применяется.
* Как работает IoC контейнер в ASP.NET Core (Transient, Scoped, Singleton)?
* Какие виды dependency injection есть? (ctor, property, method injections)
* Зачем придумали async\await, в чём бенефит асинхронного программирования? Как работает async\await под капотом?
* Что такое abstract class и interface?
* Что такое Thread pool и зачем он нужен? Какие нюансы с ним есть (сколько их на старте, что бывает когда треды закончились в пуле)?
* Зачем нужен ConfigureAwait(false)?
* Что быстрее, синхронный метод или его асинхронный вариант? При прочих равных.
* Зачем нужны Span<T>, Memory<T>, IMemoryOwner, MemoryPool<T>? В чём отличие от MemoryStream?
* В чём отличине между Func и Expression? Когда в LINQ передаётся предикат Func, а когда Expression? Для чего используется Expression?
* Сколько Heaps есть в приложении? (Small Object heap - Gen0, Gen1, Gen2), Large Object Heap (Gen2), Pinned Object Heap)

GC
* Как работает GC, как огранизована память в .NET приложении? (механизм поколений и 3 стадии - marking, relocating, compacting)
* Как может утекать память в .NET приложении? (подписка на события, неосвобождение ресурсов)
* Если есть объект А и объект Б и они ссылаются друг на друга, то они вечно живут в куче?

Примитивы синхронизации
* Что такое SpinLock (mutual exclusion lock primitive where a thread trying to acquire the lock waits in a loop repeatedly checking until the lock becomes available.)
* Mutex
* Semaphore
* reference type Synchronization block (sync block) and why it's used in lock()
* Дедлоки приложения, с чем работал на практике, объясни что такое дедлок.
* Что такое volatile, какие инструкции генерирует компилятор для процессоров при использовании volatile? (запрет компилятору и процессору по перемещению операций с переменной в коде, гарантия last possible value в переменной - иногда доходит до остановки запросов в других процессорах с этой переменной)
