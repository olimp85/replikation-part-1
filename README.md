# Репликация и масштабирование. Часть 1 - Семериков Алексей

# Задание 1
Из лекции я понял что репликации master-master отличается от master-slave тем что в первом случае репликация идет в обе стороны(то есть на оба сервера) а во втором репликация идет в одну сторону.


# Задание 2
это задание выполнял на яндекс клауд. после установки севрвера и клиента MySQL и изменения пароля и пользователя получил на мастере позицию реплецирования
![](https://github.com/olimp85/replikation-part-1/blob/main/master%20position.jpg)

Затем изменил файл сонфигурации на обоих машинах.
![](https://github.com/olimp85/replikation-part-1/blob/main/my.cnf%20vm1.jpg)
![](https://github.com/olimp85/replikation-part-1/blob/main/my.cnf%20vm2.jpg)

После этих манипуляций на slave машине ввел команду на реплицирование masterа  и запуска репликации.
![](https://github.com/olimp85/replikation-part-1/blob/main/slave%20info.jpg)

когда все запустилось,я проверил какие есть базы даннных
![](https://github.com/olimp85/replikation-part-1/blob/main/data%20bases.jpg)

Ну и для проверки я создал тестовую базу данных olimp на mastere и проверил появилась ли она на slave
![](https://github.com/olimp85/replikation-part-1/blob/main/olimp%20db.jpg)
