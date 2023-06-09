<h1 align="center">Hi there, I'm Vitaliy
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">SkillFactory student, поток PDEV-22 🇷🇺</h3>

![Typing SVG](https://readme-typing-svg.herokuapp.com?color=%2336BCF7&lines=Проект+WorldNews+модуль+D9)

<hr>
<p>Для сокрытия логинов и паролей работы приложения был использован файл <b>.env</b></p>
<p>Для подключения переменных из окружения <b>.env</b> был установлен модуль <b>python-dotenv</b></p>
<h4>Описание файла  <b>.env</b> с переменными внутри него:</h4>

<b>`DEFAULT_USER_EMAIL`</b> = 'Ваш настроенный почтовый ящик откуда будет происходить рассылка'<br>
<b>`EMAIL_USER_PASSWORD`</b> = 'Пароль от вашего email'<br>
<b>`EMAIL_HOST_USER`</b> = 'username вашего  email'<br>
<b>`WORLD_NEWS_HOST`</b> = 'http://127.0.0.1:8000'
<hr>

<h3>Важно!</h3>
<b>settings.py</b><br>

- В качестве **smpt** использовался: <b>`EMAIL_HOST`</b> = 'smtp.yandex.ru'<br>
- Порт: <b>`EMAIL_PORT`</b> = '465'
- Используйте разные email для рассылки почты и для подписки на категории
- Для упрощения регистрации пользователя установлен параметр: <b>`ACCOUNT_EMAIL_VERIFICATION`</b> = 'optional'

<hr>
<h3>P.S.</h3>

- возможность подписки реализована в деталях новостей (news/id)
- из БД таблицы <b>Subscribers</b> удалены все подписчики т.к. для теста необходимо создать своих с реальным <b>email</b>
- для проверки работы приложения рекомендуется зарегистрироваться под существующим <b">email</b>
- для создания временных email без регистрации можно использовать ресурс https://getnada.com/
- войти под своим именем и нажать кнопку <b>"стать автором"</b>
- подписаться на категории статей
- создать пост с выбранными категориями и на указанный <b>email</b> при регистрации придет письмо с кратким содержанием поста
- периодическая рассылка постов на email реализована в <b>runapscheduler.py</b> (один раз в неделю - все новости за неделю)
- для активации периодической рассылки постов необходимо ввести команду: <b>`python manage.py runupscheduler`</b>

