# Домашнее задание к занятию 10.4 «Резервное копирование» - Рыженко Назарий


---

### Задание 1

В чём разница между:

- полным резервным копированием,
- дифференциальным резервным копированием,
- инкрементным резервным копированием.

*Приведите ответ в свободной форме.*

Понятно без слов

![image](https://user-images.githubusercontent.com/106932460/219873285-755005b8-2de0-4334-837f-c2513f2e1678.png)

![image](https://user-images.githubusercontent.com/106932460/219873308-b2c421fc-68a6-40cd-9ea5-0ece2eca0557.png)

![image](https://user-images.githubusercontent.com/106932460/219873264-67e29834-2ce8-4643-ae5c-48dc120922ec.png)

---

### Задание 2

Установите программное обеспечении Bacula, настройте bacula-dir, bacula-sd,  bacula-fd. Протестируйте работу сервисов.

*Пришлите конфигурационные файлы для bacula-dir, bacula-sd,  bacula-fd.*

![image](https://user-images.githubusercontent.com/106932460/220160335-8ad3d685-fab3-4a51-b128-5f1caa396983.png)

[bacula-dir](bacula-dir.conf)
[bacula-sd](bacula-sd.conf)
[bacula-fd](bacula-fd.conf)

---

### Задание 3

Установите программное обеспечении Rsync. Настройте синхронизацию на двух нодах. Протестируйте работу сервиса.

*Пришлите рабочую конфигурацию сервера и клиента Rsync.*

![image](https://user-images.githubusercontent.com/106932460/220169052-853bd982-ad6c-488f-a12d-9307ab6854af.png)

[BASH скрипт](backup-node1.sh)
[rsyncd.conf](rsyncd.conf)
[rsyncd.scrt](rsyncd.scrt)


---

### Задание со звёздочкой*
Это задание дополнительное. Его можно не выполнять. На зачёт это не повлияет. Вы можете его выполнить, если хотите глубже разобраться в материале.

---

### Задание 4*

Настройте резервное копирование двумя или более методами, используя одну из рассмотренных команд для папки /etc/default. Проверьте резервное копирование.

*Пришлите рабочую конфигурацию выбранного сервиса по поставленной задаче.*

Rsync

Инкрементное работает корректно, только я думал, что новые файлы будут сохранятся в папку incremental, а не в current, зачем тогда папка incremental?

![image](https://user-images.githubusercontent.com/106932460/220198235-f87add3e-3de2-40dc-8271-56bb4770338a.png)

![image](https://user-images.githubusercontent.com/106932460/220197403-de89542e-3cc6-4b03-87c2-fe36b5a74960.png)

![image](https://user-images.githubusercontent.com/106932460/220198361-195f708b-c0ea-4f29-a537-ba0303a316bc.png)

Bacula

