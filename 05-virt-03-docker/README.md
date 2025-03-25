# Задача 1

https://hub.docker.com/repository/docker/myashnew2/custom-nginx/general

# Задача 2

!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task2.jpg)

# Задача 3

При нажатии Ctrl-C - nginx останолвился. Это не корректная комбинация для выхода. 

У нас возникает проблема что мы изменили порт внутри контейнера, но не изменили конфигурацию на хостовой машине - перенаправление с 8080 продолжает работатать на порт 80, а контейнер ожидает поступление запроса на новом порту 81

!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task%203%20Container%20bash%20.jpg)
!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task%203%20port%20change%2080to81.jpg)

# Задача 4

!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task%204%20p1.jpg)
!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task%204%20p1.jpg)
# Задача 5 

!(https://github.com/Myash-New/05-virt-03-docker/blob/main/Task5%20%20.jpg)
И выполните команду "docker compose up -d". Какой из файлов был запущен и почему? Docker Compose автоматически выбрал файл compose.yaml, так как он имеет более высокий приоритет. В результате был запущен сервис Portainer.
