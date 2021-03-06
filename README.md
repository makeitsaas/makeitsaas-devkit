# Make it SaaS - Dev Kit

Contains all tier services (daemons, admin tools) for local development. What it does :

* Redis server (port `6379` by default)
* MySQL server (port `3306` by default)
* Mongo server (port `27017` by default)
* PhpMyAdmin (port `8080` by default)
* Mongo Express (port `8081` by default)
* Redis-commander (port `8082` by default)
* *todo* : health checker
* *todo* : api gate (http.s + ws.s) + editor
* *todo* : Jupyter

These ports will be open by default. Their values can be changed by editing `docker-compose.yml` file. If you do this,
you will have to update `.env` values in project services (other repositories).

## Getting started

By default, if all you local ports are available, you can just clone this repo and start docker compose :

```
git clone https://github.com/makeitsaas/makeitsaas-devkit devkit
cd devkit
docker-compose up -d
```

## Stop 

As usual :

```
docker-compose stop && docker-compose rm -f
```
