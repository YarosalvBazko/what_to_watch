### Как запустить проект:

## Клонировать репозиторий и перейти в него в командной строке:

```bash
git clone 
```

```bash
cd what_to_watch
```

## Cоздать и активировать виртуальное окружение:

```bash
python3 -m venv venv
```

```bash
source venv/bin/activate
```
#### или для пользователей Windows

```bash
source env/Scripts/activate
```

## Установить зависимости из файла requirements.txt:

```bash
python3 -m pip install --upgrade pip
```

```bash
pip install -r requirements.txt
```

## Запустить проект:

```bash
flask run
```