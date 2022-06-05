# Внутренний проект компаний **Y_lab**

## Для запуска проекта, выполните следующие шаги:

1. Создайте своего собтсвенного бота https://telegram.me/BotFather

2. Создайте виртуальное окружение:
```bash
python -m venv env
```

3. Войдите в виртуальное окружение:
```bash
source env/bin/activate
```

4. Установите зависимости:
```bash
pip install -r requirements.txt
```

5. Скопируйте файл с переменными окружения:
```bash
cp .env.example .env
```

6. В файле `.env` установите в переменную `BOT_TOKEN`, токен своего созданного бота.
```
BOT_TOKEN=...
```

7. В файле `bot.py` измените код в конце на:

![Такой](README.assets/start.png)

8. Попросите у команды файл `credentials.json`.
netstat -pna | grep 6379
## Сборка образов и запуск контейнеров

В корне репозитория выполните команду:
```bash
docker-compose up --build -d
```
При первом запуске данный процесс может занять несколько минут.

### Остановка контейнеров
Выполните команду:
```bash
docker-compose stop
```
### Настройка commit-hook
Установите pre-commit вне виртуального окружения:
```bash
pip install pre-commit
```
