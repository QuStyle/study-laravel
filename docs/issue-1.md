# Инициализация ларавел

## Добавить alias на инсталятор laravel/installer
1. Заходим в контейнер php `docker exec -it php sh` и устанавливаем alias
    ```shell
        alias laravel="/home/www-data/.composer/vendor/bin/laravel"
    ```

## Установка фреймворка

1. Проверяем что директории src внутри контейнера доступна на запись. Если нет, IDE в корне проекта выполнить команду `sudo chmod 777 ./src`
2. Заходим в контейнер php `docker exec -it php sh` и выполняем действие `laravel new example-app`
3. Переносим все файлы с директории example-app в корень директории src `mv ./example-app/* ./ && ./.* ./`