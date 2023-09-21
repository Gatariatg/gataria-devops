## string connect mongodb

srv://gataria-tg:minhamae@cluster0.djihq0c.mongodb.net/?retryWrites=true&w=majority

## Runnin gataria via docker

docker run --name backend-catalog -e MONGO_DATABASE="dev" -e MONGO_URL="mongodb+srv://gataria-tg:minhamae@cluster0.djihq0c.mongodb.net/" -p 3010:3010 -d gataria-backend-catalog-dev2

docker run -d --name backend-images -e CATAPI_URL="https://api.thecatapi.com/v1/images/search" -p 3020:3020 gataria-backend-images-dev

docker run -d --name frontend -p 3000:3000 gataria-frontend:dev 