<h3>Подключение к MySql</h3>
Для подключения к базе данных необходимо использовать в качестве адреса сервера
название сервиса MySql, по-умолчанию название <b>mysql</b>
<br>
Пароль <b>root</b> пользователя указывается в <b>.env</b> файле в переменной 
<b>MYSQL_ROOT_PASSWORD</b>
<h3>Настройка SSL</h3>
SSL настраивается автоматически при запуске <b>docker-compose.yml</b>
<br>
Для избежания ошибки небезопасного соединения необходимо добавить 
корневой сертификат <b>rootCA.pem</b> в доверенные сертификаты системы, это трелбуется сделать
только один раз, все сертификаты выдаваемые контейнером <b>Nginx</b> создают их на основе
корневого сертефиката