Чтобы проверить образы, загруженные в GitHub и Docker, выполните:

1)Выберите образ,который хотите установить локально.

2)Скачайте образ с GHCR на вашу локальную машину с помощью команды: 

docker pull ghcr.io/9e8is/shorturl-service:latest

docker pull ghcr.io/9e8is/shorturl-service:latest.

3)Установленные образы можно запустить командами: 

docker run -d -p 8000:80 -v todo_data:/app/data todo-service:latest 

docker run -d -p 8001:80 -v shorturl_data:/app/data shorturl-service:latest

Установка с Docker.

1)Запустите контейнер с образом можно командой:

docker run -d -p 8000:80 denis22/todo-service:latest

docker run -d -p 8001:80 denis22/shorturl-service:latest
