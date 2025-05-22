# Инициализация ларавел

## Добавить alias на инсталятор laravel/installer
1. Заходим в контейнер php `docker exec -it php sh` и устанавливаем alias
    ```shell
        alias laravel="/home/www-data/.composer/vendor/bin/laravel"
    ```

## Установка фреймворка

1. Заходим в контейнер php `docker exec -it php sh` и выполняем действие `laravel new example-app`