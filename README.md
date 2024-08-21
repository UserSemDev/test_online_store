<h3 align="center">Проект: Тестовое задание</h3>

## О проекте

Онлайн платформа торговой сети электроники

## Технологии

- [![Python](https://img.shields.io/badge/Python-092E20?style=flat&logo=Python)](https://www.python.org/)
- [![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=Django)](https://www.djangoproject.com/)
- [![Django REST Framework](https://img.shields.io/badge/Django%20REST%20Framework-092E20?style=flat)](https://www.django-rest-framework.org/)
- [![PostgreSQL](https://img.shields.io/badge/PostgreSQL-092E20?style=flat&logo=PostgreSQL)](https://www.postgresql.org/)

## Задание

- Создайте веб-приложение с API-интерфейсом и админ-панелью.
- Создайте базу данных, используя миграции Django

## Настройка проекта

Для работы с проектом произведите базовые настройки.

### 1. Клонирование проекта

Клонируйте репозиторий используя следующую команду.

  ```sh
  git clone https://github.com/UserSemDev/test_online_store.git
  ```

### 2. Настройка виртуального окружения и установка зависимостей

- Инструкция для работы через виртуальное окружение - poetry:

```text
poetry init - Создает виртуальное окружение
poetry shell - Активирует виртуальное окружение
poetry install - Устанавливает зависимости
```

### 3. Редактирование .env.sample:

- В корне проекта переименуйте файл .env.sample в .env и отредактируйте параметры:
    ```text
    # Postgresql
    POSTGRES_ENGINE="postgresql_psycopg2" - используем psycopg
    POSTGRES_DB="db_name" - название вашей БД
    POSTGRES_USER="postgres" - имя пользователя БД
    POSTGRES_PASSWORD="secret" - пароль пользователя БД
    POSTGRES_HOST="host" - можно указать "localhost" или "127.0.0.1"
    POSTGRES_PORT=port - указываете порт для подключения по умолчанию 5432
    
    # Django
    SECRET_KEY=secret_key - секретный ключ django проекта
    DEBUG=True - режим DEBUG

### 4. Настройка БД:

- Примените миграции:
  ```text
  python manage.py migrate
  ```
- Наполнение данными БД из фикстур:
  ```text
  python manage.py loaddata $(ls fixtures/)
  ```

## Использование

### Для запуска проекта наберите в терминале команду:

  ```text
  python manage.py runserver
  ```

перейдите по адресу: [http://127.0.0.1:8000](http://127.0.0.1:8000)


### Документация проекта

Swagger: http://127.0.0.1:8000/swagger/

## Контакты

Ссылка на репозиторий: [https://github.com/UserSemDev](https://github.com/UserSemDev)