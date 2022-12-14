[[Ethernet]]*** - тоже тут!
Он уютно расположился на 1 и 2 уровнях модели OSI

----------------
Сети делятся на локальные (LAN — Local Area Network) и глобальные (WAN — Wide Area Network). Локальными сетями принято называть сети, которые используются в зданиях, школах и организациях. Глобальными считают сети в масштабах города, страны, континента.

К локальным сетям предъявляли простые требования: одни должны были объединять все сетевые устройства предприятия, предоставлять достаточную пропускную способность и быстродействие.

Для удовлетворения этих требований было разработано несколько технологий LAN: Token Ring, FDDI, Ethernet.

Token Ring и FDDI использовали кольцевую топологию и были сложны в реализации. Поэтому и были вытеснены другой технологией — Ethernet, которая до сих пор используется и развивается.

----------
Ethernet описывается стандартами группы IEEE 802.3 и работает на канальном уровне. Данная технология непрерывно развивалась и на данный момент имеет следующие стандарты:

-   Ethernet  10BASE-T со скоростью передачи данных 10Мбит/с по витой паре 3-й категории  и выше.
-   [[Fast Ethernet]]  100BASE-T со скоростью передачи данных 100Мбит/с по витой паре 5-й категории.
-   Gigabit Ethernet 1000BASE-T со скоростью передачи данных 1000Мбит/с по витой паре 5-й категории.
-   10 Gigabit Ethernet 10GBASE-T со скоростью передачи данных 10 Гбит/с по витой паре 6-й категории.

--------------------
### А что это за категории такие?

Категории описывают характеристики кабеля для передачи данных на большой скорости. Чем выше категория, тем лучше характеристики.

### А можно использовать и другие кабели?

Конечно. Это всего лишь часть стандартов. Существуют и стандарты для передачи по оптическим кабелям. Максимальная длина между 2-мя устройствами составляет 100 м при передачи по кабелям UTP/STP. UTP/STP кабели представляют собой симметричный кабель, состоящий из 4 скрученных между собой пар (медных проводников). Для вышеописанных стандартов используются только 2 пары для связи. В технологиях 1000BASE-T и 10GBASE-T используются все 4 пары.

[Урок 12. Краткое описание технологии и стандартов Ethernet (easy-network.ru)](https://easy-network.ru/22-urok-12.html)


### А как  работает Ethernet?

Ethernet изначально разрабатывалась с общей средой передачи данных и использовала топологию типа [[Общая шина]] (Bus). То есть в любой момент времени только одно устройство могло осуществлять передачу. Если 2 и более устройств начинали передачу, то возникала коллизия, которая не позволяла сети нормально функционировать. Поэтому была придумана технология, которая бы в определенной степени управляла процессом — [[CSMA CD]] (Carrier Sense Multiple Access with Collision Detection) множественный доступ с контролем несущей и обнаружением коллизий. Благодаря данной технологии каждому устройству выделялось ограниченное время для передачи данных.

-----------
В настоящее время в данной технологии нет необходимости, так как для каждого устройства выделяется свой канал передачи. Достигается это благодаря коммутаторам. Кроме того, это позволяет устройствам работать в дуплексном режиме. Работу [[коммутатор]] мы подробно рассмотрим в одном из следующих уроков.

--------------
Как мы уже знаем Ethernet используется на канальном уровне. При поступлении [[пакет]]а данных с сетевого уровня на канальный к пакету добавляется специальный заголовок. Рассмотрим структуру кадра. Существуют 4 типа кадра, которые отличаются дополнительными полями. В этом уроке мы рассмотрим тип кадра Ethernet II, так как он и используется с [[протокол IP]] .

-----------
![[Pasted image 20221109133950.png]]

_**Преамбула**_ — своего рода метка  начала кадра, чтобы сетевые устройства могли знать где заканчивается один кадр и начинается другой.


-------
_**Адрес получателя**_ — [[MAC-адрес]] получателя, то есть адрес устройства, для которого и предназначен данный кадр.

--------
_**Адрес отправителя**_ — [[MAC-адрес]]-адрес отправителя, то есть адрес устройства, отправившего данный кадр.
(Поскольку линия Ethernet передает сообщение в соответствии с порядком байтов "Big Endian" (т. Е. Старший байт передается первым, см. Соответствующий документ для порядка байтов), а порядок битов - "Little Endian" (т.е. есть младший бит передается первым)). Итак, есть следующая картинка (слева для передачи):)