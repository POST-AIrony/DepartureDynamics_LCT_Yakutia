# DepartureDynamics

![DepartureDynamics Logo](link/to/logo.png)

**Проект "DepartureDynamics" разработан командой "Oaks Dungeon" с целью предоставления сервиса по анализу вероятности увольнения сотрудников на основе статистики электронных писем.**

## О проекте

DepartureDynamics — это инновационный сервис, который использует машинное обучение и анализ электронных писем для предсказания вероятности увольнения сотрудников. Проект включает в себя парсинг электронных писем, обучение собственной модели на основе статистических данных и визуализацию результатов предсказаний.

## Основные характеристики

- **Цели проекта:**
  - Анализ вероятности увольнения сотрудников.
  - Парсинг электронных писем сотрудников для сбора статистических данных.
  - Обучение собственной модели машинного обучения для предсказания вероятности увольнения.
  - Визуализация результатов предсказаний модели.

- **Технологии и инструменты:**
  - Бэкенд (API): Реализован на FastAPI.
  - Модель машинного обучения: Используется CatBoost.
  - Фронтенд (веб-интерфейс): Разработан с использованием HTML, CSS и JS.
  - Парсинг электронных писем: Реализован с использованием библиотек imap и email.
  - База данных: Используется PostgreSQL с использованием библиотеки Ormar.

## Установка

### Локальная установка

1. Склонируйте репозиторий:

   `git clone https://github.com/OaksDungeon/DepartureDynamics_LCT_Yakutia`

2. Перейдите в директорию проекта:

   `cd DepartureDynamics_LCT_Yakutia/server`

3. Установите зависимости:

   `pip install -r requirements.txt`

4. Запустите приложение:

   `uvicorn app:app --reload`

   Приложение будет доступно по адресу [http://127.0.0.1:8000](http://127.0.0.1:8000).

### Онлайн-версия

Вы также можете использовать [онлайн-версию](http://89.232.176.235:8000/main) проекта для удобного взаимодействия с функциональностью сервиса.

## Использование

### API

Проект предоставляет API с различными возможностями, включая:
- Регистрацию и аутентификацию пользователя.
- Управление моделями машинного обучения.
- Выполнение предсказаний на основе модели.
- Парсинг электронных писем.
- Получение информации о текущем пользователе и многое другое.

Для подробной документации по API посетите [ссылку](http://89.232.176.235:8000/docs/api/index).

### Веб-интерфейс



## База данных

Проект использует PostgreSQL для хранения данных. В базе данных содержатся следующие основные таблицы:

- **Таблица `users_db`:**
  - Содержит информацию о пользователях, включая их идентификатор, дату создания, статус администратора, имя, фамилию, адрес электронной почты и хэшированный пароль.

- **Таблица `feedback`:**
  - Хранит обратную связь от пользователей, включая уникальный идентификатор, дату создания, имя пользователя, адрес электронной почты и сообщение.

- **Таблица `models`:**
  - Содержит информацию о моделях, связанных с пользователями. Включает уникальный идентификатор, дату создания, дату обновления, тип модели, путь к данным, название модели, путь к файлу модели и идентификатор пользователя.

- **Таблица `history`:**
  - Сохраняет историю действий пользователей, включая уникальный идентификатор, дату создания, дату обновления, имя файла с прогнозами, прогнозы пользователя, название прогноза и идентификатор пользователя.

- **Таблица `parse_history`:**
  - Хранит информацию о процессе разбора данных пользователей, включая уникальный идентификатор, дату создания, дату обновления, начальную и конечную даты базового периода, начальную и конечную даты сравнительного периода, время начала и окончания рабочего дня, путь к данным, путь для сохранения результатов и идентификатор пользователя.



## Контакты

- **Чесников Леонид** (Ai-Engineer & Project-manager)
- **Какой-то Алексей** (Backend)
- **Тронев Алексей** (Design)
- **Сорокина Александра** (Frontend)
- **Какой-то Тимофей** (Frontend)

## Лицензия

Проект распространяется под лицензией [MIT](LICENSE).
