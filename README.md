# Website

## Bringing Up the Web Service

`docker compose up`

Force a rebuild: `docker compose up --build`

## Building a Distribution

### Compile the App

`docker exec -it angular-ui npm run build`

### Copy Files Out of Docker

`docker cp angular-ui:/app/dist/web ~/Downloads`

Afterwards, upload the contents of the `web` folder into an S3 Bucket

## Shutting Down

`docker compose down`
