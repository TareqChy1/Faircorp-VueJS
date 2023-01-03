# Faircorp Vue.js

## Docker

#### Build Docker Image

Build the Docker image with docker build command in the terminal:
```bash
docker build -t docker-img-vuejs .
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
docker run -it -p 8081:8080 -d - name docker-vuejs faircorp/docker-img-vuejs
```
- -it  –  This flag sets the container in Interactive mode and allocate a Dedicated TTY id for later SSHing.

- -d –  This flag sets the container to run in the background.

- -p 8081:8080 – Port Forwarding Between Host and the Container. Right to the colon is a container and Left to the colon is Host. 8081 is the Host and 8080 is the container Port.

- –name – Once started docker daemon assigns a random string name to the container. But I recommend defining a name can be a handy way to add meaning to a container.

- docker-vuejs – Name of the container we are starting ( Replacement of Container ID).

- faircorp/docker-img-vuejs – The name of the image from which we are going to create a Container.


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
