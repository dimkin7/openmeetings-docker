# openmeetings-docker

Используя контейнер https://hub.docker.com/r/apache/openmeetings#! создать файл docker-compose.yml и выполнить разворачивание данного сервиса, с использованием сети типа MACVlan с возможностью подключения к сервису из локальной сети. Данные сервиса, хранимые в БД сервиса перенести на том VOLUME.

Том должен быть создан в папке /home/user/project/

https://github.com/openmeetings/openmeetings-docker

---
Запуск:
docker-compose build
docker-compose up

docker-compose down
Журнал
docker-compose logs -f openmeetings

Войти в bash контейнера
docker-compose exec openmeetings bash
или
docker exec -it openmeetings-docker-openmeetings-1 bash


Узнать IP ("ip a" не работает)
hostname -I | awk '{print $1}'
172.19.0.2
Тест 
https://172.19.0.2:5443/
http://172.19.0.2:5080

Регистрация
dima-besh
!1Qwerty
---



Поднять сервисы в контейнерах, чтобы взаимодействовать с камерами.
Сохранять данные в отдельных volume, чтобы можно менять с хостовой машины.
Поднять сеть macvlan, чтобы оборащаться с хостовой машины, снаружи.
Скриншот на хостовом компьютере, где показано, что есть доступ до сервиса.
