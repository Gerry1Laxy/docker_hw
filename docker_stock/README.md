## Docker stock

Сборка образа выполняется из текущей директории репозитория с помощью команды:

```shell
$ docker build -t stock-dock .
```

Запустить контейнер с помощью команды:

```shell
$ docker run --name stock-dock-server -d -p 8081:80 stock-dock
```
