# Docker Lab 2

Практическая работа по Docker, Docker Compose и Git.

## Описание

Проект представляет собой простое fullstack-приложение To-Do List.

В состав проекта входят три сервиса:

- frontend — Nginx, отдаёт HTML-страницу и проксирует API-запросы;
- backend — Python Flask API для работы с задачами;
- postgres — база данных PostgreSQL для хранения задач.

## Запуск

Перед запуском нужно создать файл .env на основе .env.example:

## docker compose down -v
При docker compose down данные сохраняются, потому что именованный volume postgres_data не удаляется.
При docker compose down -v Docker удаляет volume postgres_data, поэтому файлы PostgreSQL исчезают, и после нового запуска база создаётся заново пустой.