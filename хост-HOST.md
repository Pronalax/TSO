Как узнать количество **хостов** в **сети**?

**Количество** **хостов** **в** подсети = 2n-2, где n – это **количество** свободных бит (нулей) в порции **хоста**, а «-2» - это вычет адреса **сети** (в порции **хоста** все нули) и широковещательного адреса (в порции **хоста** все единицы). Объяснение формул расчета **сетей**.

----------------------------------------------------------------------
![[Pasted image 20221107223112.png]]
Там еще все зависит от [[маска сети]] 


![[Pasted image 20221108025831.png]]



![[Pasted image 20221108025626.png]]

/24 - 24 битная маска 11111111.11111111.11111111.00000000
- кол-во хостов(компьютер в 1 подсети) - [Cisco формула расчёта сетей (infocisco.ru)](https://infocisco.ru/cisco_formula_subnetting.html)
