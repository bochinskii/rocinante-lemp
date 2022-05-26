<h1>Проект "Rocinante LEMP" на AWS EC2 Instance'е</h1><br>
<p>
С помощью GitHub Action - "lemp" устанавливается LEMP с CMS Drupal 9.
</p>
<p>
В директории "configs" находятся необходимые конфигурационные файлы и TLS сертификат
для HTTPS. С помощью данного action'а и переменной REAL_KEY экспортируется TLS ключ
сайта для HTTPS.
</p>
<p>
Файлы в корне диретории необходимы для создания ec2 instance'а.
</p>
<p>
 GitHub Action - "Add_configs" - это пример альтернативной доставки конфигураций на сервер.
</p>
<p>
Вот какие "секреты" тут есть:<br>
<br>
GH_ACTION_ACCESS_KEY_ID - ключ доступа к AWS;<br>
GH_ACTION_SECRET_ACCESS_KEY - секретный ключ доступа к AWS;<br>
<br>
SSH_KEY - SSH ключ для доступа к ec2 инстансу;<br>
SSH_PORT - кастомный SSH порт;<br>
<br>
REAL_KEY - ключ валидного сертификата;<br>
<br>
MYSQL_ROOT_PASS - root пароль для базы данных;<br>
<br>
MYSQL_ADMIN_USER - имя администратора mysql;<br>
MYSQL_ADMIN_USER_PASS - пароль администратора;<br>
<br>
MYSQL_DRUPAL_DB - база данных сайта;<br>
MYSQL_DRUPAL_USER - пользователь базы данных сайта;<br>
MYSQL_DRUPAL_USER_PASS - пароль пользователя базы данных сайта;<br>
<br>
SITE_DIR - префикс директории с сайтом;
</p>
<p>
Status of our Actions:
</p>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/lemp/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Add_configs/badge.svg?branch=main"><br>
<br>
<p>
Denis Bochinskii
</p>
