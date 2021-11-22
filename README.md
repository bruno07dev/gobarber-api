<h1 align="center">
  <img alt="Logo" src="src/assets/logo.png" width="200px">
</h1>

<h3 align="center">
  ✂️ Express Application for Gobarber project
</h3>

<p align="center">An app for your barbershop!</p>

<p align="center">
  <a href="#%EF%B8%8F-about-the-project">About the project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-technologies">Technologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-getting-started">Getting started</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-how-to-contribute">How to contribute</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-license">License</a>
</p>

## 📝 About the project

The provider can manage your appointments and receive notification when a new appointment is scheduled, also see if one client canceled the schedule.

The client can list all providers, see their available times and schedule or cancel a service.

To see the **App Client**, click here: [GoBarber Rest API](https://github.com/bruno07dev/appgobarber)</br>
To see the **Web client**, click here: [GoBarber App](https://github.com/bruno07dev/webgobarber)</br>

## 🛠 Technologies

Technologies that I used to develop this api

- [Node.js](https://nodejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/)
- [Multer](https://github.com/expressjs/multer)
- [TypeORM](https://typeorm.io/)
- [JWT-token](https://jwt.io/)
- [uuid v4](https://www.npmjs.com/package/uuidv4)
- [PostgreSQL](https://www.postgresql.org/)
- [Date-fns](https://www.npmjs.com/package/date-fns)
- [Jest](https://jestjs.io/)
- [Supertest](https://www.npmjs.com/package/supertest)
- [Husky](https://github.com/typicode/husky)
- [Commitlint](https://github.com/conventional-changelog/commitlint)
- [Commitizen](https://github.com/commitizen/cz-cli)
- [Eslint](https://eslint.org/)
- [Prettier](https://prettier.io/)
- [EditorConfig](https://editorconfig.org/)

## 💻 Getting started
**Import the Insomnia.json on Insomnia App**

### Requirements

```bash
Node.js
Yarn or npm
One instance of PostgreSQL
Docker
Insomnia
```

**Clone the project and access the folder**

```bash
$ git clone https://github.com/bruno07dev/gobarber-api.git && cd gobarber-api
```

**Follow the steps below**

```bash
# Install the dependencies
$ yarn

# Make a copy of '.env.example' to '.env'
# and set with YOUR environment variables.
# The aws variables do not need to be filled for dev environment
$ cp .env.example .env

# Create the instance of postgreSQL using docker
$ docker run --name gobarber-postgres -e POSTGRES_USER=docker \
              -e POSTGRES_DB=gobarber -e POSTGRES_PASSWORD=docker \
              -p 5432:5432 -d postgres

# Create the instance of mongoDB using docker
$ docker run --name gobarber-mongodb -p 27017:27017 -d -t mongo

# Create the instance of redis using docker
$ docker run --name gobarber-redis -p 6379:6379 -d -t redis:alpine

# Once the services are running, run the migrations
$ yarn typeorm migration:run

# To finish, run the api service
$ yarn dev:server

Well done, project is started!
```

## How to contribute 🤝

**Make a fork of this repository**

```bash
# Fork using GitHub official command line
# If you don't have the GitHub CLI, use the web site to do that.

$ gh repo fork bruno07dev/gobarber-api
```
**Follow the steps below**

```bash
# Clone your fork
$ git clone your-fork-url && cd gobarber-api

# Create a branch with your feature
$ git checkout -b my-feature

# Make the commit with your changes
$ git commit -m 'feat: My new feature'

# Send the code to your remote branch
$ git push origin my-feature
```

After your pull request is merged, you can delete your branch

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

> Status Project: Project finalized :heavy_check_mark:
# 🎬 Desenvolvedores

[<img src="https://avatars.githubusercontent.com/u/66931016?s=460&u=68bdaab4339d594139e0f083a0346b30ddb8402d&v=4" width=115 > <br> <sub> Bruno Cardoso </sub>](https://www.linkedin.com/in/bruno-s-cardoso/) |
| :---: |

Made with 💜 by Bruno Cardoso 👋
