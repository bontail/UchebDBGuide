### Как установить дамп с гелиоса на локальный компьютер

1. Скачать [файл](./ucheb_db_dump) к себе на компьютер

2. Если PostgreSQL установлен локально на компьютере, то ~~пересмотрите взгляды на жизнь~~ пропускайте этот шаг<br>

   a) Запустите docker container [(compose file)](./docker-compose.yml)<br>

   b) Скопируйте container_id (docker ps)<br>

   c) docker cp ./ucheb_db_dump **[container_id]**:/ucheb_db_dump<br>

3. psql -X postgres < ucheb_db_dump