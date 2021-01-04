#  SECURE MERN STACK SERVICES - DOCKER NGINX REVERSE-PROXY PROJECT

:school: This DOCKER MERN STACK SERVICES is a project school MBA 2st promotion :books:

## **🎬 Description**

Includes 2 microservices :

Authentification (Sign-up & Login) securised with jwt

Posting articles (List, Edit handling)

<br/>

## **🧱 Structure**

In folder server and client we will find a Dockerfile to build the image:

> ./backend/auth-api/Dockerfile
> ./backend/products-api/Dockerfile
>
> ./frontend/Dockerfile

In main repository we will find a docker-compose.yml to set containers launching:

> ./docker-compose.yml

<br/>

## **⚙️ Setup Composing**

Dockerfile content:

> **FROM**: Use a lighter version of Node as a parent image
>
> **WORKDIR**: Set the working directory
>
> **COPY**: Copy the current directory contents into the container at /api
>
> **RUN**: install dependencies
>
> **EXPOSE**: Make port XXXX available to the world outside this container
>
> **CMD**: Run the app when the container launches

In docker-compose.yml:

_we will find there the version and the services of deployment_

<br/>

## **:rocket: Install & Deployment**

> :\$ git clone https://github.com/Jekdesign/valsin_jerry_si2_2020_securite.git

Use docker:

> :\$ **docker-compose up --build** or **docker-compose up -d --build**
>
> _Shutdown if necessary: :\$ docker-compose down_

<br/>

Pactical basic for npm package manager

> ###### First, run the backend
>
> :\$ cd backend/auth-api/ and backend/products-api/
>
> :\$ npm install
>
> :\$ npm start
>
> ###### Then, run the frontend
>
> :\$ cd frontend/
>
> :\$ npm install
>
> :\$ npm start

<br/>

:memo: Note

Connection db `mongodb://mongodb:27017/db-auth` and `mongodb://mongodb:27017/db-products`

Backend : auth-api port `https://localhost:3001` and products-api port `https://localhost:3002`

Client access `https://localhost:3000`

<br/>

## **💻 Technologies**

**Mongodb** _(database)_

**Express** _(node.js framework)_

**React** _(front js framework)_

**Node** _(tool javascript environment)_

**Docker** _(CGROUP + Namespace)_

**CGROUP** _(Partitioning ressources - system, memory, networks)_

**Namespace** _(Insulation for the creation of a container)_

<br/>