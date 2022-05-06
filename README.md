<h1>Проект "Rocinante LEMP"</h1><br>
<p>
С помощью GitHub Action - Deploy_lemp_auto устанавливается LEMP с CMS Drupal 9. Происходит это на основе user data скрипта - user.data.sh.raw. С помощью данного action'а определяются все необходимые переменные и данный файл в base64 кодировке используется при разворачивании LEMP.
</p>
<p>
С помощью GitHub Action's - Add_configs (или add_configs_v2) происходит тонкая настройка сервисов, путем добавление или изменения конфигурационных файлов. Так же, данный action обеспечивает "заливку" валидного ключа сертификата, который находится в определенном секрете. Сам сертификат (real_rocinante.cert) находится в открытом доступе в директории проекта.
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
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Deploy_lemp_auto/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/add_configs_v2/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Add_configs/badge.svg?branch=main"><br>
<br>
<p>
Denis Bochinskii
</p>
