для сисмона:

[](https://stackoverflow.com/posts/55855400/timeline)

Идентификатор GUID сам по себе ничего не означает. Его цель состоит в том, чтобы позволить вам коррелировать и фильтровать события процесса, когда Windows повторно использует идентификаторы процессов (таким образом, вы можете думать о нем как о совершенно уникальном идентификаторе процесса).

От:[https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)

«Включает идентификатор GUID процесса в события создания процесса, чтобы обеспечить корреляцию событий даже при повторном использовании Windows идентификаторов процессов»









GUID технически означает глобальный уникальный идентификатор. На самом деле это 128-битная структура, которая_вряд ли_когда-либо повторится или создаст столкновение. Если вы делаете математику, область значений находится в[ундециллионах](https://en.wikipedia.org/wiki/Names_of_large_numbers#Standard_dictionary_numbers).

Используйте идентификаторы GUID, если у вас есть несколько независимых систем или клиентов, создающих идентификаторы, которые должны быть уникальными.

Например, если у меня есть 5 клиентских приложений,([[клиентское приложение]]) создающих и вставляющих транзакционные данные в таблицу с уникальным ограничением на идентификатор, используйте идентификаторы GUID. Это предотвращает необходимость принудительного запроса клиентом сначала выданного идентификатора с сервера.

Это также отлично подходит для фабрик объектов и систем, которые имеют множество типов объектов, хранящихся в разных таблицах, где вы не хотите, чтобы 2 объекта имели один и тот же идентификатор. Это значительно упрощает реализацию схем кэширования и очистки.


------------------

Идентификаторы GUID используются при разработке программного обеспечения в качестве ключей базы данных, компонента идентификаторы или практически везде В противном случае по-настоящему уникальным идентификатором является Обязательно. Идентификаторы GUID также используются для идентификация всех интерфейсов и объектов в ПРОГРАММИРОВАНИЕ COM.
