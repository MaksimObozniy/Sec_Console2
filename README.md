Sec_Console2
===

Описание проекта
---
"Sec_Console2" - это система управления доступом, которое позволяет отслеживать входы и выходы с объекта. 
Проект разработан на Python (3.11.4) и использует Django (3.2.25) для создания веб-интерфейса.

Функциональность
---
1. Отображение активных пропусков: Список всех активных пропусков которые могут быть использованы для входа на объект.
2. Просмотр информации о пропуске: Подробная информация о каждом пропуске, включая историю посещений.
3. Информация о посещениях: Данные о посещениях, когда и кто использовал пропуск для входа и выхода с объекта.

Установка
-----
1. Клоинруйте репозиторий:
```bash
git clone https://github.com/MaksimObozniy/Sec_Console2.git
```

2. Перейдите в каталог проекта и выполните команду для усановки виртуального окружения:
```bash
python -m venv .venv
```

3. Установите необходимые зависимости:
```bash
pip install -r requirements.txt
```

4. Создайте файл .env для работы с секретными данными (Секретные ключи, подключение к базе данных)

   В нем необходимо будет написать настройки для поделючения к базе данных:
   DB_NAME = Имя базы данных
   DB_USER = Имя пользователя базы данных
   DB_PASSWORD = Пароль пользователя
   DB_HOST = Это параметр настройки, который используется для указания адреса сервера базы данных в проекте.
   DB_PORT = Это параметр, который указывает на порт, через которое приложение будет подключаться к серверу базы данных.
   SECRET_KEY = Это большое случайное число, применяемое для защиты от CSRF. Важно, чтобы ключ, используемый в продакшене, не указывался в исходном коде, и/или не запрашивался с другого сервера.
   ALLOWED_HOSTS = Это настройка в файле settings.py в Django, которая определяет список доменных имен или IP-адресов, с которых разрешено обслуживать ваше приложение.
   
5.Запустите сервер разработки
```bash
python manage.py runserver
```

Использование
----
Откройте веб-браузер и перейдите по адресу "http://127.0.0.1:8000/", чтобы начать работу с приложением "Sec_Console2".

