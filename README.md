<h1>Проект "Rocinante LEMP"</h1><br>
<br>
<p>
С помощью GitHub Action - Deploy_lemp_auto устанавливается LEMP с CMS Drupal 9. Происходит это на основе user data скрипта - user.data.sh.raw. С помощью данного action'а заменяются все необходимые переменные и данный файл в base64 кодировке используется при разворачивании LEMP.
</p>
<p>
С помощью GitHub Action - Add_configs (add_configs_v2) происходит тонкая настройка сервисов, путем добавление или изменения конфигурационных файлов.
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
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Deploy_lemp_auto/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/add_configs_v2/badge.svg?branch=main"><br>
<img src="https://github.com/bochinskii/rocinante-lemp/workflows/Add_configs/badge.svg?branch=main"><br>
<p>
Denis Bochinskii
</p>
