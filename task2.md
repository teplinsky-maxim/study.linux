## 2

1. 512 байт, состоит из:
    * Кода загрузки
    * 4 записи для загрузки
    * Сигнатуры загрузчика

2. Вообще 4, но разделы можно также помещать в расширенные части MBR
3.  BIOS:
	- Стартуем из ROM
	- POST
	- Настройка шин и переход в 16-разрядный режим
	- Загрузка системы

	UEFI:
	- Security Phase
	- Pre-EFI Initialization
	- Driver Execution Environment
	- Boot Device Select
	- Transient System Load
	- Runtime

4. sysvinit: 
    - Установка права на запись для группы и остальные биты в `umask`
    - Происходит системный вызов `reboot()` с параметром `RB_DISABLE_CAD` для ядра, чтобы послать 
    `SIGINT` процессу с pid'ом 1
    - `ioctl()` с `KDSIGACCEPT` и `SIGWINCH` процессу с pid'ом 1
    - Закрытие всех i\o потоков (stdin, stdout, stderr)
    - `PATH` ->  `/sbin:/usr/sbin:/bin:/usr/bin`
    - Создание `/var/run/utmp` с правами 0644
    - Инициализация `inittab`
    - Вызов `init` 
    - Выяснение текущего runlevel'a по умолчанию (либо запрос его у юзера)
    
    systemd: 
    - вызов `default.target`
    - вызов тасков из `/etc/systemd/system/multi-user.target.wants`
    - вызов `sysinit.target`
    - вызов `local-fs.target`
    - вызов остальных всех тасков
    
5. ![Скрин системы](sysd.png?raw=true)
6. Каталог или файл, с помощью которого обеспечивается доступ к новой файловой системе, каталогу или файлу
7. Регулярный файл
8. `pwd`
9. `cp -R <src> <dst>`
10. `touch`, `mkdir`
11. /root
