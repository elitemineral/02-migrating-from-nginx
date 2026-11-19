# Миграция с nginx

В репозитории располагается конфиг Angie.
Для работоспособности необходимо

1. Установить пакет angie-module-brotli

```
sudo apt install -y angie-module-brotli
```

2. Создать симлинк на конфиг дефолтного сервера

```
sudo ln -s /etc/angie/sites-available/default /etc/angie/sites-enabled/default
```

3. Проверить сайт, выполнив команду

```
curl -I localhost:8080
```