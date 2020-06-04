# Infrastructure Project 

That is the **docker-compose part** of full stack project consisting of (at least) 4 Docker Containers 
started with docker-compose file
- database container (postgres)
- database user interface container (pgadmin4)
- [backend container (spring boot)](https://github.com/val3ri/springboot-project-template)
- [frontend container (angular)](https://github.com/val3ri/angular-project-template)

You need the docker-compose.yml from this project to build this multiple container application.

**the structure should like this** (some of the important files are on the picture below):

```
fullstack-project-folder
└───backend folder
│   │   ...
│   └───src
│       │   ...
│   
└───frontend folder
│   └───nginx
│   │   │   default.conf
│   │
│   │   proxy-config-local.json
│   │  ...
│
└───infrastructure folder 
│   │   README.md
│   │   docker-compose.yml
```

## Used technologies
- Angular
- Docker
- Spring Boot
- nginx
- npm
- Maven

## Required Software for starting the the application
- [Angular cli](https://cli.angular.io/)
- [Docker](https://www.docker.com/products/docker-desktop)
- [Maven](https://maven.apache.org/)
- [npm](https://www.npmjs.com/get-npm)

## Steps for "prod" deployment
- building the angular project - production files
```
ng build 
```
creates the **dist** folder in the angular project

- building spring boot jar
```
mvn package
```
that is the command line solution, but you can also do it straight with your IDE

- open the folder of the infrastructure project with the console and:
```
docker-compose up
```
that will startthe multiple container application, creating all of the 4 containers (only if you already create the right project structure like in the picture above!)

## Steps for running the the backend or/and frontend application/s locally
work in progress :writing_hand:

## info about: database - postgres
work in progress :writing_hand:	

## info about: database user interface - pgadmin4
work in progress :writing_hand:	

## info about: backend - spring boot
work in progress :writing_hand:	

## info about: frontend - angular 
work in progress :writing_hand:	