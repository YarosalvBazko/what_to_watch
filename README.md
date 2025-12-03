# What to Watch

Веб‑приложение для хранения и просмотра мнений о фильмах. Позволяет добавлять новые отзывы, просматривать случайные мнения и получать доступ к конкретным записям по ID.

## Функционал

- Добавление мнений о фильмах (название, текст отзыва, ссылка на обзор).
- Просмотр случайного мнения на главной странице.
- Просмотр конкретного мнения по ID.
- Загрузка данных из CSV‑файла через CLI‑команду.
- Обработка ошибок 404 и 500 с пользовательскими шаблонами.
- Валидация данных (обязательные поля, уникальность текста отзыва).
##
## Структура проекта
```bash
what_to_watch/
├── instance/
│   └── db.sqlite3              # База данных SQLite
├── migrations/                 # Миграции базы данных (Flask-Migrate)
├── opinions_app/
│   ├── static/                 # Статические файлы (CSS, JS, изображения)
│   ├── templates/              # HTML-шаблоны
│   ├── cli_commands.py         # CLI-команды
│   ├── error_handlers.py       # Обработчики ошибок
│   ├── forms.py               # Формы WTForms
│   ├── __init__.py            # Инициализация приложения
│   ├── models.py              # Модели SQLAlchemy
│   └── views.py               # View-функции (маршруты)
├── .env                       # Переменные окружения
├── .gitignore               # Список игнорируемых файлов
├── opinions_app.py          # Основной файл приложения
├── opinions.csv             # Пример данных для загрузки
├── README.md               # Документация
├── requirements.txt          # Зависимости
└── settings.py              # Настройки приложения
```

## Требования

- Python 3.9+
- SQLite (для локальной разработки)
- pip (для установки зависимостей)
##

## Установка и запуск

### Клонируйте репозиторий:
```bash
git clone https://github.com/YarosalvBazko/what_to_watch.git
```
```bash
cd what_to_watch
```

### Создайте и активируйте виртуальное окружение:
#### Для macOS/Linux:
```bash
python3 -m venv venv
```
```bash
source venv/bin/activate
```
### Для Windows:
```bash
python -m venv venv
```
```bash
venv\Scripts\activate
```
### Установите зависимости:
```bash
python -m pip install --upgrade pip
```
```bash
pip install -r requirements.txt
```
### Запустите приложение:
```bash
flask run
```
### Приложение будет доступно по адресу: http://127.0.0.1:5000

