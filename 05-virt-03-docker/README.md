# Задача 1

https://hub.docker.com/repository/docker/myashnew2/custom-nginx/general

# Задача 2

!(https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task2.jpg))

# Задача 3

При нажатии Ctrl-C - nginx останолвился. Это не корректная комбинация для выхода. 

У нас возникает проблема что мы изменили порт внутри контейнера, но не изменили конфигурацию на хостовой машине - перенаправление с 8080 продолжает работатать на порт 80, а контейнер ожидает поступление запроса на новом порту 81

https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task%203.jpg

# Задача 4

https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task%204.jpg
# Задача 5 

https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task5%20%20.jpg
https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task5%20%20p1.jpg
https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task5%20%20p2.jpg
https://github.com/Myash-New/Netology-SHDEVOPS-17/blob/main/05-virt-03-docker/Task5%20%20portainer%20.jpg


И выполните команду "docker compose up -d". Какой из файлов был запущен и почему? Docker Compose автоматически выбрал файл compose.yaml, так как он имеет более высокий приоритет. В результате был запущен сервис Portainer.
