Flask Blog — Мой Блог: Достижения и Навыки
Коротко
Этот небольшой проект — учебный Flask-блог, демонстрирующий основы шаблонов, статических файлов и стилизации с помощью HTML/CSS. В проекте есть страница с описанием навыков, профильным изображением и таблицей прогресса по темам курса.
Особенности
•	Простое Flask-приложение с одним маршрутом ("/") и использованием render_template.
•	HTML-шаблон содержит более 10 разных HTML-тегов (header, nav, main, section, article, figure, img, table и др.).
•	CSS подключён через url_for('static', filename='style.css') и задаёт фон, шрифты, размеры текста и расположение компонентов.
•	Таблица на 8 колонок и 4 строки заполнена в соответствии с заданием.
Структура проекта
flask-blog/
├── app.py
├── requirements.txt
├── README.md
├── templates/
│ └── index.html
└── static/
    ├── style.css
    └── avatar.jpg
Установка (локально)
1.	Склонируйте репозиторий:
git clone <ВАША-ГИТХАБ-ССЫЛКА>
2.	Перейдите в папку проекта:
cd flask-blog
3.  Создайте виртуальное окружение и активируйте его:
python -m venv venv
•	Windows: venv\Scripts\activate
•	macOS / Linux: source venv/bin/activate
4.	Установите зависимости:
pip install -r requirements.txt
Файл requirements.txt
Пример содержимого:
flask==3.0.3

Запуск приложения
1.	Запустите приложение:
python app.py
2.	Откройте в браузере:
http://127.0.0.1:5000/
Описание ключевых файлов
•	app.py — минимальный Flask-приложение, создаёт экземпляр Flask и маршрут "/", возвращающий render_template("index.html").
•	templates/index.html — основной HTML-шаблон. Содержит секции: intro, skills, achievements (таблица). Использует {{ url_for('static', filename='...') }} для подключения CSS и изображения.
•	static/style.css — стилизация страницы: фон (градиент), шрифты, размеры текста, оформление карточек и таблицы.
•	static/avatar.jpg — изображение.