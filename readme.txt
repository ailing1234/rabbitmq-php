1. Install erlang
2. Install rabbitmq
3. Start the rabbitmq service.
4. Open browser and login to rabbitmq.
url: http://localhost:15672/#/queues
username: guest
password: guest

5. Install composer

6. Add extension=php_sockets.dll into php.ini in your php installation directory such as c:\xampp\php. 
Restart your apache service.

7. In terminal,
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '55ce33d7678c5a611085589f1f3ddf8b3c52d662cd01d4ba75c0ee0459970c2200a51f492d557530c71c15d8dba01eae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"

8. Interminal,
composer require php-amqplib/php-amqplib

9. Create send.php
10. Create receive.php
11. In terminal:
php send.php
php receive.php