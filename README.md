# Как запустить проект

## Порядок выполнения команд
1. Запустить докер контейнеры `docker compose up -d`
2. Заходим в контейнер php `docker exec -it php sh` и устанавливаем alias для доступности консольной утилиты laravel
    ```shell
        alias laravel="/home/www-data/.composer/vendor/bin/laravel"
    ```
3. Если ОС линус, добавить в /etc/hosts запись 
    ```shell
        127.0.0.1 laravel.test
    ```
4. Перейти в браузере по ссылке http://laravel.test