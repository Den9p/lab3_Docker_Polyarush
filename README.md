# lab3_Docker_Polyarush
По заданию необходимо было разбить на 3 образа (бд-мастер, реплика, тгБот), однако я решил так не делать т.к это без надобности, Dockerfile для настройки бд мне не пригодились, реплика настроена в docker-compose.yaml, также необходимо учесть что для сборки проекта нужен .env в директории /tgbot

Для монтирования .env используется Dockerfile поэтому файл .env должен быть внутри /tgbot
