# Strapi application

A quick description of your strapi application

## Docker commands

**To export a backup from docker**
```shell
docker exec -t react-avancado-api_postgres_1 pg_dumpall -c -U strapi > dump_`date +%d-%m-%Y"_"%H_%M_%S`.sql
```

**To import a backup to docker**
```shell
cat strapi.sql | docker exec -i react-avancado-api_postgres_1 psql -U strapi
```
