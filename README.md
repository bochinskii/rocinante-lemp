<h1>Проект "Rocinante LEMP"</h1><br>
<br>
<p>
С помощью GitHub Action - Deploy_lemp происходит установка LEMP с установленной CMS Drupal 9. Происходит это на основе user data скрипта, который находится в "секрете" - USER_DATA_SCRIPT. Файл user_data.sh.raw - это шаблон данного user data скрипта.
</p>
<p>
С помощью GitHub Action - Add_configs происходит тонкая настройка сервисов, путем добавление или изменения конфигурационных файлов.
</p>
<p>
Так же, после установки lemp происходит "заливка" сертификатов для HTTPS
</p>
<p>
Вот какие "секреты" тут есть:<br>
GH_ACTION_ACCESS_KEY_ID - ключ доступа к AWS;<br>
GH_ACTION_SECRET_ACCESS_KEY - секретный ключ доступа к AWS;<br>
SSH_KEY - SSH ключ для доступа к ec2 инстансу;<br>
SSH_PORT - кастомный SSH порт;<br>
USER_DATA_SCRIPT - user data скрипт в base64 формате;<br>
REAL_KEY - ключ сертификата, который будет в продакшене (сам сертификат находится в корне проекта);<br>
</p>
<p>
Status of our Actions:
</p>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Deploy_lemp/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Add_configs/badge.svg?branch=main"><br>
<p>
Denis Bochinskii
</p>
