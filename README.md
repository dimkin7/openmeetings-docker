# openmeetings-docker

Используя контейнер https://hub.docker.com/r/apache/openmeetings#! создать файл docker-compose.yml и выполнить разворачивание данного сервиса, с использованием сети типа MACVlan с возможностью подключения к сервису из локальной сети. Данные сервиса, хранимые в БД сервиса перенести на том VOLUME.

Том должен быть создан в папке /home/user/project/


Поднять сервисы в контейнерах, чтобы взаимодействовать с камерами.

Сохранять данные в отдельных volume, чтобы можно менять с хостовой машины.

Поднять сеть macvlan, чтобы оборащаться с хостовой машины, снаружи.
