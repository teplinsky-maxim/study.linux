## Oсновные принципы Unix-way
1.  _Красиво — небольшое._
2.  _Пусть каждая программа делает что-то одно, но хорошо._
3.  _Стройте прототип программы как можно раньше._
4.  _Предпочитайте переносимость эффективности._
5.  _Храните данные в простых текстовых файлах._
6.  _Извлекайте пользу из уже существующих программных решений._
7.  _Используйте  для уменьшения трудозатрат и улучшения переносимости._
8.  _Избегайте пользовательских интерфейсов, ограничивающих возможности пользователя по взаимодействию с системой._
9.  _Делайте каждую программу «фильтром»._

---

2. Линус Торвальдс является разработчиком ядра Linux
3. `uname -a`
4.  19:40:52 up  2:06,  0 users,  load average: 0.52, 0.58, 0.59
* 19:40:52 - текущее время
* up  2:06 - время работы системы
* 0 users - кол-во текущих юзеров
* load average: 0.52, 0.58, 0.59 - средняя загрузка системы для последних 1, 5 и 15 минут

5. `df -h`
6. ```
	Procs
	    r: The number of processes waiting for run time.
	    b: The number of processes in uninterruptible sleep.
	Memory
	    swpd: the amount of virtual memory used.
	    free: the amount of idle memory.
	    buff: the amount of memory used as buffers.
	    cache: the amount of memory used as cache.
	    inact: the amount of inactive memory. (-a option)
	    active: the amount of active memory. (-a option)
	Swap
	    si: Amount of memory swapped in from disk (/s).
	    so: Amount of memory swapped to disk (/s).
	IO
	    bi: Blocks received from a block device (blocks/s).
	    bo: Blocks sent to a block device (blocks/s).
	System
	    in: The number of interrupts per second, including the clock.
	    cs: The number of context switches per second.
	CPU
	    These are percentages of total CPU time.
	    us: Time spent running non-kernel code. (user time, including nice time)
	    sy: Time spent running kernel code. (system time)
	    id: Time spent idle. Prior to Linux 2.5.41, this includes IO-wait time.
	    wa: Time spent waiting for IO. Prior to Linux 2.5.41, included in idle.
	    st: Time stolen from a virtual machine. Prior to Linux 2.6.11, unknown.
7.

* Ядро: `Linux DESKTOP-KOB9FR5 4.4.0-19041-Microsoft #488-Microsoft Mon Sep 01 13:43:00 PST 2020 GNU/Linux`
* Архитектура : `x86_64`
* SSD: `382G`
* ОЗУ: `16696316 kB` = `16GB`
* Средняя нагрузка: `0.5`

---
Git поставил путем `sudo apt install git`

![system](/scr.png?raw=true)
