#### ПРО ПИНГ

Теперь про **ping**. Можно сказать, это самый базовый инструмент инженера, который позволяет понять “"А жив ли хост?"

Помимо прочего, пинг поможет понять как долго пакет доходит до адреса назначения и, соответственно, поможет измерить задержку.

Работает ping предельно просто:

1.  Источник отправляет запрос вида **ICMP echo request**. Это выглядит как вопрос “бро, ты живой?"
2.  Получатель отправляет ответ источнику **ICMP echo reply**. Это звучит как ответ вида “да, бро, я жив, спасибо!"
3.  Время с момента отправки вопроса до получения ответа суммируется и считается за время пинга

![[Pasted image 20221108140817.png]]

эта утилита, которая используется в [[ICMP]] 