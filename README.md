# Parking Control API

Spring Boot project base on [Michelle Brito Tutorial](https://www.youtube.com/watch?v=LXRU-Z36GEU)

## Tech Stack
* JDK 17
* Spring Boot 2.6.3
* Postgres 14.2

## Dependencies
* Spring Web
* Spring Data JPA
* Validation
* PostgreSQL Driver

## Running the API
First create a directory at the project's root level `pgdata` and run:
```
$ docker-compose up -d
```
Then start the API with the follow:
```
$ ./mvnw spring-boot:run
```


## Endpoints
```
GET http://localhost:8080/parking-spot?page=0&size=5&sort=registrationDate,DESC

GET http://localhost:8080/parking-spot/uuid

POST http://localhost:8080/parking-spot

PUT http://localhost:8080/parking-spot/uuid

DELETE httpp://localhost:8080/parking-spot/uuid
```