# Faircorp Vue.js

## Docker

#### Build Docker Image

Build the Docker image with docker build command in the terminal:
```bash
docker build -t vuejs-docker .
```
Here the PERIOD/DOT at the end is intentional and it represents the current directory.  With this command issued, Docker looks for a Dockerfile in the current directory and create the image out of it.

#### To validate if your image has created
To know the list of images available in your system locally. use the following command.
```bash
docker images
```

#### Run Docker Image
Run Docker image using given command:
```bash
docker run -it -p 8080:8080 --rm --name docker-vuejs vuejs-docker

```



## Project setup

```
npm install
```

### Compiles and hot-reloads for development

```
npm run serve
```

### Compiles and minifies for production

```
npm run build
```

### Lints and fixes files

```
npm run lint
```
