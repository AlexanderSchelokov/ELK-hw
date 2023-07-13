Задание 1. Elasticsearch
---
Установите и запустите Elasticsearch, после чего поменяйте параметр cluster_name на случайный.

Приведите скриншот команды 'curl -X GET 'localhost:9200/_cluster/health?pretty', сделанной на сервере с установленным Elasticsearch.

**Ответ**

![Снимок](https://github.com/AlexanderSchelokov/ELK-hw/assets/121572590/f6363657-cd58-406d-b25d-6bfae9cd8fe3)

***

Задание 2. Kibana
---

Установите и запустите Kibana.

Приведите скриншот интерфейса Kibana на странице http://<ip вашего сервера>:5601/app/dev_tools#/console, где будет выполнен запрос GET /_cluster/health?pretty.

**Ответ**

![Снимок1](https://github.com/AlexanderSchelokov/ELK-hw/assets/121572590/06d8ae06-424e-49b2-a224-ad12f435a9df)

***

Задание 3. Logstash
---

Установите и запустите Logstash и Nginx. С помощью Logstash отправьте access-лог Nginx в Elasticsearch.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx.

**Ответ**

![Снимок6](https://github.com/AlexanderSchelokov/ELK-hw/assets/121572590/fe324522-1144-40d2-b5ac-897db37213f8)

***



Задание 4. Filebeat.
Установите и запустите Filebeat. Переключите поставку логов Nginx с Logstash на Filebeat.

Приведите скриншот интерфейса Kibana, на котором видны логи Nginx, которые были отправлены через Filebeat.

Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже шире разобраться в материале.

Задание 5*. Доставка данных
Настройте поставку лога в Elasticsearch через Logstash и Filebeat любого другого сервиса , но не Nginx. Для этого лог должен писаться на файловую систему, Logstash должен корректно его распарсить и разложить на поля.
