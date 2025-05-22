# Shorty - Сервис сокращения URL

Shorty - это современный сервис для сокращения длинных URL-адресов, состоящий из двух частей: бэкенд на Python и фронтенд на React с TypeScript.

## Репозитории проекта

- **Бэкенд**: [github.com/kalibdune/shorty-backend](https://github.com/kalibdune/shorty-backend)
- **Фронтенд**: [github.com/kalibdune/shorty-frontend](https://github.com/kalibdune/shorty-frontend)

## Обзор проекта

Shorty позволяет пользователям создавать короткие, удобные ссылки вместо длинных URL-адресов. Сервис предоставляет веб-интерфейс для управления ссылками и API для интеграции с другими системами.

### Основные функции

- Сокращение длинных URL-адресов
- Генерация QR-кодов для сокращенных ссылок
- Отслеживание количества кликов по ссылкам
- Управление личными ссылками через аккаунт пользователя
- Автоматическое копирование сокращенных ссылок в буфер обмена

## Архитектура проекта

### Бэкенд (Python)

- Python 3.12+
- Poetry для управления зависимостями
- База данных с использованием Alembic для миграций
- RESTful API для взаимодействия с фронтендом

### Фронтенд (React + TypeScript)

- React с TypeScript
- Webpack для сборки
- Поддержка мобильных устройств
- Современный UI с интуитивно понятным интерфейсом

## Запуск проекта

### Использование Docker

Самый простой способ запустить проект - использовать Docker Compose:

```bash
git clone https://github.com/username/shorty.git
cd shorty
docker-compose up
```

После запуска:
- Фронтенд будет доступен по адресу: http://localhost:80
- Бэкенд API: http://localhost:8000

### Локальный запуск для разработки

#### Бэкенд:

```bash
cd shorty-backend
poetry install
poetry shell
python -m shorty
```

#### Фронтенд:

```bash
cd shorty-frontend
npm install
npm run dev
```

Фронтенд в режиме разработки будет доступен по адресу: http://localhost:5050
