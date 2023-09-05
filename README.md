# sentry 9.1.2
Sentry environment

One of the last lightweight sentry service

Before launching Sentry you should make `.env` from `.env.sample` and fill out the credentials inside the `.env` file.

`cp .env.sample .env`

To launch Sentry run the command:

```
docker-compose up -d
docker-compose exec -ti web sentry upgrade
docker-compose exec -ti web pip install sentry-plugins
docker-compose restart
```
