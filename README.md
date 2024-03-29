# Домашнее задание к занятию «Кеширование Redis/memcached» Шарапат Виктор

### Задание 1. Кеширование 

Приведите примеры проблем, которые может решить кеширование. 

*Приведите ответ в свободной форме.*

### Решение 1
Кеширование может помочь решить следующие проблемы:
1) Увеличение производительности: Кеширование позволяет ускорить доступ к данным, так как данные сохраняются в кеше и могут быть быстро извлечены, вместо того чтобы каждый раз обращаться к источнику данных (например, базе данных или удаленному API).
2) Снижение нагрузки на сервер: Кеширование позволяет снизить количество запросов к серверу, так как часть данных уже доступна в кеше, что уменьшает нагрузку на сервер.
3) Улучшение масштабируемости: Кеширование может помочь улучшить масштабируемость системы, так как уменьшает нагрузку на серверы и базы данных, позволяя им обрабатывать больше запросов.
4) Улучшение отзывчивости приложения: Загрузка данных из кеша обычно быстрее, чем запрос к серверу, что может улучшить отзывчивость приложения для конечных пользователей.
5) Снижение издержек на доступ к внешним ресурсам: Кеширование может помочь уменьшить издержки на доступ к внешним ресурсам, таким как удаленные API или сервисы.
---

### Задание 2. Memcached

Установите и запустите memcached.

*Приведите скриншот systemctl status memcached, где будет видно, что memcached запущен.*

### Решение 2

sudo apt update

sudo apt install memcached

sudo systemctl start memcached

sudo systemctl status memcached

![alt text](https://github.com/sharvik22/11-02.md/blob/main/images/1.png)

---

### Задание 3. Удаление по TTL в Memcached

Запишите в memcached несколько ключей с любыми именами и значениями, для которых выставлен TTL 5. 

*Приведите скриншот, на котором видно, что спустя 5 секунд ключи удалились из базы.*

### Решение 3
Я установил параметр TTL = 20, т.к. при значении 5, значение записи быстро удаляется и поэтому не выводится результат, точнее от пустой.  

![alt text](https://github.com/sharvik22/11-02.md/blob/main/images/6.png)


---

### Задание 4. Запись данных в Redis

Запишите в Redis несколько ключей с любыми именами и значениями. 

*Через redis-cli достаньте все записанные ключи и значения из базы, приведите скриншот этой операции.*

### Решение 4
![alt text](https://github.com/sharvik22/11-02.md/blob/main/images/9.png)
![alt text](https://github.com/sharvik22/11-02.md/blob/main/images/10.png)

---

## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже разобраться в материале.


### Задание 5*. Работа с числами 

Запишите в Redis ключ key5 со значением типа "int" равным числу 5. Увеличьте его на 5, чтобы в итоге в значении лежало число 10.  

*Приведите скриншот, где будут проделаны все операции и будет видно, что значение key5 стало равно 10.*

### Решение 5

![alt text](https://github.com/sharvik22/11-02.md/blob/main/images/11.png)
