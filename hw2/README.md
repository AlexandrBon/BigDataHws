## Описание частей дз
### Part 1
Hadoop кластер развернут в следующей конфигурации: 1 namenode, 1 datanode, 1 resourcemanager, 1 nodemanager. 
Поднятие сервисов было с помощью докер-файла с практики: https://github.com/smalyshevv/bigdata-docker-pyspark/blob/main/docker-compose.yaml

Рассмотрим картинку с выполненными тасками в `Spark`:
![Screenshot](spark_tasks.png)

На каждый `read` потребовалось по 1 стэйджу(3 чтения, одно тестовое). На `count()` потребовалось по 2 стэйджа, т.к. нужна операция `shuffle`.