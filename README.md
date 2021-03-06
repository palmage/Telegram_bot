# Учебный проект: Telegram-bot проверки статуса домашней работы

## Описание проекта
Бот-асcистент используется для оповещения об изменения статуса домашней работы на курсе Яндекс.Практикум через мессенджер Telegram.
Для мониторинга статуса ДР бот опрашивает API Яндекс.Практикум.

Сообщения от бота:

* У вас проверили работу "<homework_name>"!  
  К сожалению в работе нашлись ошибки.
* Работу "<homework_name>" взяли на ревью!
* У вас проверили работу "{homework_name}"!  
  Ревьюеру всё понравилось, можно приступать к следующему уроку.

## Требования
![](https://img.shields.io/badge/python-v3.7-blue)

## Как развернуть
1. Склонируйте репозиторий: ```https://github.com/palmage/telegram_bot```.
2. С помощью [инструкции](https://python-scripts.com/virtualenv) создайте и активируйте виртуальное окружение.
3. Установите зависимости: ```pip install -r requirements.txt```.
4. Добавьте файл `api_sp1_bot/.env` и внесите в него переменные окружения:
```PowerShell
TELEGRAM_TOKEN = '<telegram_token>'
TELEGRAM_CHAT_ID = '<telegram_chat_id>'
PRAKTIKUM_TOKEN = '<yandex_prakticum_token>'
```
5. Запустите программу: ```python homework.py```.
