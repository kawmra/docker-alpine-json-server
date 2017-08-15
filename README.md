# Download

```
$ git clone https://github.com/kawmra/docker-alpine-json-server
```

# Setup

Define your data to `/data/db.json` and define custom routing rule to `/data/routes.json` for [json-server](https://github.com/typicode/json-server).

# Build

Build json-server and json-server-data images.

```
$ docker-compose build
```

# Run

Run json-server and json-server-data contaienrs.

```
$ docker-compose up -d
```

Specify `-d` to run in detach mode.

# Access

Open http://localhost:3000/ in your browser.

# Stop and remove

Stop and remove the containers and volumes.

```
$ docker-compose down -v
```

Specify `-v` to remove volumes as well.

# Change the data and routes

To apply the changed data to the server:
1. `$ docker-compose down --volumes` to down the containers and volumes.
2. `$ docker-compose build` to rebuild the images.
3. `$ docker-compose up` to up the containers and volumes.