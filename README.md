# sentry
Sentry environment

Before launching Sentry you should make `.env` from `.env.sample` and fill out the credentials inside the `.env` file.

To launch Sentry run the command:

```
docker-compose up -d
docker-compose exec -ti web upgrade
docker-compose exec -ti pip install sentry-plugins
docker-compose restart
```
