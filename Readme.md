# Spring Rest Service

## A restful Api with following HTTP features:
 - GET
 - POST
 - PUT
- DELETE

## Getting the Project

To install clone the github repository

```php
git clone https://github.com/bmehler/spring-rest-service.git
```

### Run the Application with
```bash
$ ./mvnw clean spring-boot:run
```

## Test the api with curl with json content

GET All Request
```bash
$ curl -v localhost:8080/employees
```
GET Single Request
```bash
$ curl -v localhost:8080/employees/<id>
```
POST Request
```bash
$ curl -X POST localhost:8080/employees -H 'Content-type:application/json' -d '{"name": "Samwise Gamgee", "role": "gardener"}'
````
PUT Request
```bash
$ curl -X PUT localhost:8080/employees/<id> -H 'Content-type:application/json' -d '{"name": "Samwise Gamgee", "role": "ring bearer"}'
```
Delete Request
```bash
$ curl -X DELETE localhost:8080/employees/<id>
```