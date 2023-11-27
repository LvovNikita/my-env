# Локальное окружение

## Приложения

| Приложение                  | Порт  | Пользователь | Пароль   |
|-----------------------------|-------|--------------|----------|
| PostgreSQL 13               | 5432  | postgres     | postgres |
| ClickHouse 23 (HTTP)        | 8123  |              |          |
| ClickHouse 23  (Native TCP) | 9000  |              |          |
| MongoDB                     | 27017 |              |          |
| ETCD                        | 2379  |              |          |
| RabbitMQ                    | 5672  |              |          |
| RabbitMQ Management UI      | 15672 | guest        | guest    |

* 9000-ый порт ClickHouse — для подключения через `clickhouse-client`
* RabbitMQ Management UI доступен по адресу http://localhost:15672/

## Плагины PostgreSQL

* `postgresql-13-postgis-3` — PostGIS 3 (поддержка географических объектов)
* `postgresql-13-postgis-3-scripts` — скрипты для установки PostGIS в PostgreSQL 13
* `postgresql-contrib` — средства портирования, утилиты анализа и подключаемые функции, не включённые в состав основной системы PostgreSQL

## Запуск контейнеров

```
docker compose -f "docker-compose.yml" up -d --build
```

Или с помощью плагина: RMB `docker-compose.yml` -> Compose Up

## ПО

* [Docker](https://docs.docker.com/engine/install/)
* [Docker Desktop](https://www.docker.com/products/docker-desktop/)
* [VSCode Docker plugin](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
