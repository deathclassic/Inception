# Inception

В рамках проекта необходимо настроить инфраструтуру, состояющую из различных сервисов, с помощью docker compose:
<img width="562" alt="image" src="https://user-images.githubusercontent.com/86204727/203170501-01873185-c5ad-43bd-8948-30f97ceed84b.png">

Для этого необходимо написать соответствующие докер образы и развернуты:
• Докер контейнер с NGINX (TLSv1.2 или TLSv1.3)
• Докер контейнер с WordPress + php-fpm
• Докер контейнер с MariaDB
• Разделы с базой данных и файлами WordPress
• Докер сеть, которая устанавливает связь между контейнерами

Бонусы:
* Установлен Redis для кэширования сайта
* Установлен FTP сервер для работы с контейнером WordPress
* Установлен Adminer для работы с БД

```make``` сборка проекта
```make build``` запуск контейнеров
```make down``` остановка контейнеров
```make clean``` удаление БД и файлов WordPress
```make fclean``` полная очистка конфигурации

 На выходе получаем готовый сайт на WordPress:
<img width="979" alt="image" src="https://user-images.githubusercontent.com/86204727/203172684-7f735495-218b-4097-8550-67b6c3e3e96c.png">
