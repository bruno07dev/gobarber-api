# <p align="center">✂ GoBarber, an Express aplication project<p>

## <p align="center">An app for your barbershop!<p>

# 📝 About the project

### <p align="justify">The provider can manage your appointments and receive notification when a new appointment is scheduled, also see if one client canceled the schedule.<p>

### <p align="justify">The client can list all providers, see their available times and schedule or cancel a service.<p>

# 🛠 Technologies

#### Technologies that I used to develop this api

- Node.js
- TypeScript
- Express
- Multer
- TypeORM
- JWT-token
- uuid v4
- PostgreSQL
- Date-fns
- Jest
- SuperTest
- Husky
- Commitlint
- Commitizen
- Eslint
- Prettier
- EditorConfig

# 💻 Getting started
Import the Insomnia.json on Insomnia App

#### Requirements
- Node.js
- Yarn or npm
- One instance of PostgreSQL
- Docker
- Insomnia

#### Clone the project and access the folder

$ git clone https://github.com/bruno07dev/gobarber-api.git && cd gobarber-api
Follow the steps below

# Install the dependencies
$ yarn

### Make a copy of '.env.example' to '.env'
### and set with YOUR environment variables.
### The aws variables do not need to be filled for dev environment
$ cp .env.example .env

## Create the instance of postgreSQL using docker
$ docker run --name gobarber-postgres -e POSTGRES_USER=docker \
              -e POSTGRES_DB=gobarber -e POSTGRES_PASSWORD=docker \
              -p 5432:5432 -d postgres

## Create the instance of mongoDB using docker
$ docker run --name gobarber-mongodb -p 27017:27017 -d -t mongo

## Create the instance of redis using docker
$ docker run --name gobarber-redis -p 6379:6379 -d -t redis:alpine

## Once the services are running, run the migrations
$ yarn typeorm migration:run

## To finish, run the api service
$ yarn dev:server

### 🚀 Well done, project is started!

### For testing the aplication on the terminal
$ yarn test

# How to contribute 🤝
Make a fork of this repository

### Fork using GitHub official command line
### If you don't have the GitHub CLI, use the web site to do that.

$ gh repo fork bruno07dev/gobarber-api
Follow the steps below

### Clone your fork
$ git clone your-fork-url && cd gobarber-api

### Create a branch with your feature
$ git checkout -b my-feature

### Make the commit with your changes
$ git commit -m 'feat: My new feature'

### Send the code to your remote branch
$ git push origin my-feature
After your pull request is merged, you can delete your branch

> Status Project: Finalized :heavy_check_mark:

# 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.

[<img src="https://avatars.githubusercontent.com/u/66931016?s=460&u=68bdaab4339d594139e0f083a0346b30ddb8402d&v=4" width=115 > <br> <sub> Bruno Cardoso </sub>](https://www.linkedin.com/in/bruno-s-cardoso/) |
| :---: | 

Made by bruno07dev
