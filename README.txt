Для запуска проекта необходимо:
1. Создать базу данных на хосте MySQL.
2. В файле config/db.php прописать настройки соединения с БД и имя БД
3. В файле config/params.php изменить настройки генерации тестовых данных, если это необходимо.
4. Находясь в директории проекта, запустить:
    // импорт зависимостей, необходима предварительная установка composer
    composer create-project
    // создание структуры базы
    ./yii migrate
    // заполнение базы тестовыми данными
    ./yii fill
5. Запустить web-сервер:
    php -S localhost:5555 -t web/