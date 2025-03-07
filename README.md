## Начало работы
1. Переименовать ```.env.example``` в ```.env```
2. Запустить Docker Engine ([Docker Desktop для Windows](https://docs.docker.com/desktop/install/windows-install/))
3. Запустить проект в Docker

Выполнить команду в терминале с проектом:
```
docker compose --env-file .env up --build
```
Флаг ```--build``` используется для пересборки образов

Если контейнеры не запускаются, убедитесь, что порты `3306` (MySQL) и `8080` (phpMyAdmin) не заняты другими процессами.
## Вход в phpMyAdmin
1. Перейти по ссылке
```
http://localhost:8080
```
2. Ввести логин и пароль из ```.env```
