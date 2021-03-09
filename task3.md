## 3

1. User id
2. Файлы хранят пароли в хешированном виде и некоторые сввойства, относящиеся к учетным записям этих паролей
3. root
4. `newgrp`
5. `passwd <username>`
6. `passwd <username> -x`
7.  
	- `chmod u=rwx,g=r,o=r <file>`, `chmod 744 <file>`
	- `chmod u=r,g=w,o=x <file>`, `chmod 421 <file>`
	- `chmod u=x,g=w,o=r <file>`, `chmod 124 <file>`
9. Запись и исполнение для юзера и запись для группы
10. Чтение для юзера, чтение и исполнение (заход) для группы, все для остальных
11. `chmod 312 <file>`
12.  `chmod 614 <file>` 
13. `chmod 777 <file>` 
14. `chmod 1777 <file>`

