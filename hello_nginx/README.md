## Hello nginx

Сборка образа выполняется из текущей директории репозитория с помощью команды:

```shell
$ docker build -t hello-nginx .
```

Запустить контейнер с именем `hello-nginx-server` с помощью команды:

```shell
$ docker run --name hello-nginx-server -d -p 8081:80 hello-nginx
```
