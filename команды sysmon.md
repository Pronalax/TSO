Основными аргументами, которые могут быть переданы, являются:

[SysmonCommunityGuide/configuration.md в главном · trustedsec/SysmonCommunityGuide · GitHub (turbopages.org)](https://translated.turbopages.org/proxy_u/en-ru.ru.36b5e252-637915f4-615e7523-74722d776562/https/github.com/trustedsec/SysmonCommunityGuide/blob/master/chapters/configuration.md)


-   **-i**: установить Sysmon

sysmon.exe -i [путь к файлу конфигурации]

системный администратор. -i [путь к файлу конфигурации]

-   **-c**: применить конфигурацию

sysmon.exe -c [путь к файлу конфигурации]

-   **-u**: отменить установку Sysmon

sysmon.exe -u [сила]

-   **-m**: установить манифест события (только для Windows)

sysmon.exe -м

-   **-t**: режим отладки (только для Windows)

sysmon.exe -t [путь к файлу конфигурации]

-   **-s**: Схема печати

sysmon.exe -s [версия схемы]

-   **-nologo**: не показывать логотип sysmon (только для Windows)

sysmon.exe -нолого

-   **-accepteula**: принимает лицензионное соглашение

sysmon.exe -принять

-   **--** : Сбрасывает конфигурацию по умолчанию

sysmon.exe -с --

Элементы опций под комментарием "Файл конфигурации" позволяют настраивать фильтры и параметры, относящиеся к фильтрам.

-   **-h**: алгоритм хэширования изображений. (Только для Windows)

sysmon.exe -c -h <sha1|sha2|md5|imphash|*>

-   **-r**: проверка отзыва сертификата подписи (только для Windows)

sysmon.exe -к -р

-   **-n**: отслеживать сетевые подключения для указанного процесса / процессов.

sysmon.exe -c -n [<процесс,...>]

-   **-k**: отслеживать, когда осуществляется доступ к памяти указанного процесса / процессов. (Только для Windows)

sysmon.exe -c -k [<процесс,...>]

-   **-l**: отслеживать модули (библиотеки DLL), загруженные указанным процессом / процессами. (Только для Windows)

sysmon.exe -c -k [<процесс,...>]

-   **-d** : переименовать драйвер sysmon во время установки (ограничение в 8 символов) (только для Windows)

sysmon.exe -i -c -d <имя драйвера>

> **-g** и **--dns**-переключатели перечислены, но начиная с текущей версии, они (только для Windows) не обновляют конфигурацию.

Параметры Sysmon для Linux:

Основными аргументами, которые могут быть переданы, являются:

-   **-i**: установить Sysmon

/usr/bin/sysmon -i [путь к файлу конфигурации]

-   **-c**: применить конфигурацию

/usr/bin/sysmon -c [путь к файлу конфигурации]

/ussr/bin/sysmon -u [принудительно]

-   **-s**: Схема печати

/ussr/bin/sysmon -s [версия схемы]

-   **-accepteula**: принимает лицензионное соглашение

/ussr/bin/sysmon -accepteula

-   **--** : Сбрасывает конфигурацию по умолчанию

/ussr/bin/sysmon -c --

Элементы опций под комментарием "Файл конфигурации" позволяют настраивать фильтры и параметры, относящиеся к фильтрам.

-   **-n**: отслеживать сетевые подключения для указанного процесса / процессов.

/ussr/bin/sysmon -c -n [<процесс,...>]





