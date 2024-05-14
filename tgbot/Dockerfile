# Базовый образ
FROM python:3

# Установка зависимостей
RUN apt-get update && \
    apt-get install -y python3 && \
    apt-get install -y libpq-dev && \
    apt-get clean

# Создание директории приложения внутри контейнера
RUN mkdir -p /app/tgbot

# Установка рабочей директории
WORKDIR /app/tgbot

# Копирование исходного кода приложения
COPY . .

# Установка необходимых пакетов Python
RUN pip install --no-cache-dir -r requirements.txt

# Команда для запуска бота
CMD ["python", "tgbot.py"]
