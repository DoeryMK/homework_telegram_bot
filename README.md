# homework_telegram_bot

## **Краткое описание**
python telegram bot

Данный проект является учебным. 
Цель проекта - получение навыков работы с внешним API.

### _Доступные возможности_
Telegram-бот выполняет периодический опрос API сервера домашних работ студентов.   
В случае изменения статуса домашней работы бот отправляет сообщение пользователю с указанием текущего статуса домашней работы.
Реализовано логирование ошибок. 

_Статус домашней работы может быть трёх типов:_
reviewing: работа взята в ревью;  
approved: ревью успешно пройдено;  
rejected: в работе есть ошибки, нужно поправить.  
Если домашку ещё не взяли в работу — её не будет в выдаче.

## **Требования**

flake8==3.9.2  
flake8-docstrings==1.6.0  
pytest==6.2.5  
python-dotenv==0.19.0  
python-telegram-bot==13.7  
requests==2.26.0  


## **Работа с проектом**

В консоли выполните следующие команды:

1. Клонировать проект из репозитория
```
git clone git@github.com:DoeryMK/homework_telegram_bot.git
```
или
```
git clone https://github.com/DoeryMK/homework_telegram_bot.git
```
2. Перейти в папку с проектом и создать виртуальное окружение
```
cd <имя папки>
```
```
python -m venv venv
```
или
```
python3 -m venv venv
```
3. Активировать виртуальное окружение
```
source venv/Scripts/activate
```
или
```
source venv/bin/activate
```
4. Установить зависимости из файла requirements.txt:
```
pip install -r requirements.txt
```
5. В директории проекта создать файл .env. В файле указать значение PRACTICUM_TOKEN, TELEGRAM_TOKEN, TELEGRAM_CHAT_ID.
```
PRACTICUM_TOKEN = *токен пользователя на сервере с домашкой*
TELEGRAM_TOKEN = *токен телеграм-бота*
TELEGRAM_CHAT_ID = *токен пользователя в телеграм*
```
6. Запустить файл homework.py, либо выложить проект на виртуальный сервер.
```
Авторы - DoeryMK