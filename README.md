# Приложения

| Приложение              | Порт  | Пользователь | Пароль   |
|-------------------------|-------|--------------|----------|
| PostgreSQL              | 5432  | postgres     | postgres |
| ClickHouse (HTTP)       | 8123  |              |          |
| ClickHouse (Native TCP) | 9000  |              |          |
| MongoDB                 | 27017 |              |          |
| ETCD                    | 2379  |              |          |
| RabbitMQ                | 5672  |              |          |
| RabbitMQ Management UI  | 15672 | guest        | guest    |

* 9000-ый порт ClickHouse — для подключения через `clickhouse-client`
* RabbitMQ Management UI доступен по адресу http://localhost:15672/

# Запуск контейнеров

```
docker compose -f "docker-compose.yml" up -d --build
```

Или с помощью плагина: RMB `docker-compose.yml` -> Compose Up

# UI

[Docker Desktop](https://www.docker.com/products/docker-desktop/)

# Visual Studio Code Plugin

[Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
