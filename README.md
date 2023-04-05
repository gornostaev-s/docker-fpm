Очень простой docker образ на портах для разработки на PHP.
========================
Для php используется composer.phar, сам composer не установлен в контейнер
```
(php ./composer.phar) для его использования
```

- Внутри образа PHP версии 8.1 на php-fpm.
- Проксируются запросы через nginx контейнер.
- База данных используется (Mysql 8)

Для запуска:

1) Превратить .env.example в .env ``` cp .env.example .env ```
2) Зайти в папку с докером ``` cd docker ```
3) Сбилдить контейнеры ``` docker-compose build ```
4) Поднять контейнеры ``` docker-compose up -d ```
5) Приложение будет доступно по адресу: http://localhost



