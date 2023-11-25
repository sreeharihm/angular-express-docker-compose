# angular-express-docker-compose


docker build -t angular-client:latest . //to build angular project
docker run -d --name angular-client -p 4200:4200 angular-client:latest //application run
docker stop angular-client

docker build -t express-server:dev . //to build node js server
docker run -d --name express-server -p 3000:5000 express-server:dev
docker stop express-server

docker-compose up
