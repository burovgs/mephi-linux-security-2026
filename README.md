Табельный (уникальный) номер студента: `374396`  
Операционная система: Fedora Linux

| Файл | Раздел | Описание выполненной работы |
| :--- | :---: | :--- |
| `passwd`, `shadow`, `group` | 1 | Создан пользователь `user1` (UID `1234`), включен в группу `students`, настроен срок смены пароля 90 дней (`chage -M 90 user1`). |
| `files.out` | 2.1 | Выполнен поиск всех файлов с установленным битом set-UID (`find / -type f -perm -4000`). |
| `processes.out` | 2.2 | Выполнен мониторинг процессов с `EUID = 0` и `RUID` обычного пользователя (`ps -eo ...`). |
| `stat.out` | 1, 3, 4 | Вывод команды `stat` для `/home/user1`, `/home/user1/mycat` (set-UID) и `/home/user1/mychown` (Capabilities). |
| `getcap.out` | 4 | Настроена привилегия `cap_chown=ep` для копии утилиты `/home/user1/mychown`. |
| `sudoers` | 5 | Пользователю `user1` разрешено изменять системное время через `sudo` (`/usr/bin/date`, `/usr/bin/timedatectl`). |
| `mephi-screenshot.png` | 6.1 | Скриншот терминала с уникальным номеро. |
| `history.out` | Все | Полная история выполненных команд в терминале. |
