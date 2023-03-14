
Quick start
=====

After you clone the project, you need to download the following images and paste them into the appropriate paths:

Download https://drive.google.com/file/d/1KkPHLJkNUrDCTHG1BKJt8VMgSFxUoRrp/view?usp=sharing
Path: /backend/public

Download https://drive.google.com/file/d/1KkPHLJkNUrDCTHG1BKJt8VMgSFxUoRrp/view?usp=sharing
Path: /frontend/src/assets

Copy the config files:

```shell
cp backend/.env.example backend/.env
cp frontend/src/assets/js/config.js.example frontend/src/assets/js/config.js
```

Up all the services:

```shell
docker compose --env-file ./backend/.env up -d
```

Run migrations:
```shell
docker exec ozakee-php php artisan migrate --seed
```

Backend service host:
```shell
http://localhost:8000
```

Frontend service host:
```shell
http://localhost:8001
```