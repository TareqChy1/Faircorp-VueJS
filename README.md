# Faircorp Frontend VueJS

[Deployed Frontend on EMSE Gitlab Pages](https://github.com/TareqChy1/Faircorp-VueJS)

- Author :[Tareq Md Rabiul Hossain CHY](https://www.linkedin.com/in/tareqmdrabiulhossainchy/), [Nushrat JAHAN](https://www.linkedin.com/in/nushrat-jahan-3275a9178/) and [Erfan ENFERAD](https://www.linkedin.com/in/erfan-enferad/)
- VueJS Frontend App of the 2022 Web Programing project for [M.Sc. CPS2 Web programming course](https://ci.mines-stetienne.fr/cps2/syllabus/)
- Based on [Quentin Richaud's course](https://gitlab.com/emse1/cours_js_1)

## Context

The goal of the 2022 Web Programing project is to implement a fully functional Smart Building management system (especially building, rooms, windows and heaters controllers).\
The project is composed of a [Java SpringBoot Backend server]() and a [VueJS Frontend server](https://github.com/TareqChy1/Faircorp-VueJS) interacting together. 

## Docker

#### Docker Compose installation: 

If Docker Desktop/Toolbox for either Windows or Mac installed, that means Docker Compose already have. 
If anyone are on a Linux machine, will need to [install Docker Compose](https://docs.docker.com/compose/install/). 
After installation, able to run the following and see version information.

```
docker compose version
```

#### Run docker-compose.yml file:

Firstly make sure no other copies of the app/db are running first by running following command:

```
docker ps
```

Start up the application stack using the following command. We’ll add the -d flag to run everything in the background.

```
docker compose up -d
```

We’ll notice that the volume was created as well as a network! By default, Docker Compose automatically creates a network specifically for the application stack.

Finally look at the logs using following command.
```
docker compose logs -f
```

We’ll see the logs from each of the services interleaved into a single stream. This is incredibly useful when we want to watch for timing-related issues. The -f flag “follows” the log, so will give we live output as it’s generated.


## Project setup or access :
Install all the dependencies

```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

We locally run our Faircorp_Backend project in [localhost:8080](http://localhost:8080) and Faircorp_Frontend project in [localhost:8081](http://localhost:8081) 

NB : The frontend is supposed to work with the Spring Backend deployed on Clever-Cloud. If not or if anyone want to run the backend locally, anyone can configure the API's hostname in [./src/config.js](./src/config.js)

### Compiles and minifies for production
```
npm run build
```

