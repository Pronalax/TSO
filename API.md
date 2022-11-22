Слово «API» мелькает в вакансиях даже для начинающих тестировщиков. То REST API, то SOAP API, то просто API. Что же это за зверь такой? Давайте разбираться!  
  
— А зачем это мне? Я вообще-то web тестирую! Вот если пойду в автоматизацию, тогда да… Ну, еще это в enterprise тестируют, я слышал…

- _API (Application programming interface)_ — это контракт, который предоставляет программа. «Ко мне можно обращаться так и так, я обязуюсь делать то и это».

Если переводить на русский, это было бы слово «договор». Договор между двумя сторонами, как договор на покупку машины:  
  

-   мои обязанности — внести такую то сумму,
-   обязанность продавца — дать машину.

  
Перевести можно, да. Но никто так не делает ¯\_(ツ)_/¯  
  
Все используют слово «контракт». Так принято. К тому же это слово входит в название стиля разработки:

-   Code first — сначала пишем код, потом по нему генерируем контракт
-   Contract first — сначала создаем контракт, потом по нему пишем или генерируем код (в этой статье я буду говорить именно об этом стиле)


Мы же не говорим «контракт на продажу машины»? Вот и разработчики не говорят «договор». Негласное соглашение.  
  

## API — набор функций

  
Когда вы покупаете машину, вы составляете договор, в котором прописываете все важные для вас пункты. Точно также и между программами должны составляться договоры. Они указывают, как к той или иной программе можно обращаться.  
  
Соответственно, API отвечает на вопрос “Как ко мне, к моей системе можно обратиться?”, и включает в себя:  
  

-   саму операцию, которую мы можем выполнить,
-   данные, которые поступают на вход,
-   данные, которые оказываются на выходе (контент данных или сообщение об ошибке).


![[Pasted image 20221118154451.png]]


Тут вы можете мне сказать:  
  
— Хмм, погоди. Операция, данные на входе, данные на выходе — как-то всё это очень сильно похоже на описание функции!  
  
_Если вы когда-то сталкивались с разработкой или просто изучали язык программирования, вы наверняка знаете, что такое функция. Фактически у нас есть данные на входе, есть данные на выходе, и некая магия, которая преобразует одно в другое._  
  
И да! Вы будете правы в том, что определения похожи. Почему? Да потому что API — это набор функций. Это может быть одна функция, а может быть много.