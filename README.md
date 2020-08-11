<h2 align="center">
   ♻️ NextLevelWeek 1.0 ♻️
</h2>

<p align="center">
  <a href="#computer-project">Project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-built-with">Built with</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#information_source-how-to-run">How to run</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  </p>

## :computer: Project 

 Ecoleta is an application that aims to help people find places that collect specific types of waste, encouraging people to recycle more.

## :rocket: Built with

This project was developed with the following technologies:

<details>
  <summary>Backend</summary>

-   [Node.js](https://nodejs.org/)
-   [Express](https://expressjs.com/)
-   [TypeORM](https://typeorm.io/)
-   [Typescript](https://www.typescriptlang.org/)
-   [TS-Node-Dev](https://www.npmjs.com/package/ts-node-dev)
-   [Celebrate](https://github.com/arb/celebrate)
-   [Tsyringe](https://github.com/microsoft/tsyringe)
-   [uuidv4](https://www.npmjs.com/package/uuidv4)
-   [Cors](https://www.npmjs.com/package/cors)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [VS Code](https://code.visualstudio.com/)

</details>

<details>
  <summary>Frontend</summary>

-   [React](https://pt-br.reactjs.org/)
-   [Typescript](https://www.typescriptlang.org/)
-   [Styled Components](https://styled-components.com/)
-   [Context API](https://reactjs.org/docs/context.html)
-   [React-toggle](https://github.com/aaronshaf/react-toggle)
-   [React-spring](https://www.react-spring.io/)
-   [uuidv4](https://www.npmjs.com/package/uuidv4)
-   [Axios](https://www.npmjs.com/package/axios)
-   [React Dropzone](https://github.com/react-dropzone/react-dropzone)
-   [React Icons](https://react-icons.netlify.com/#/)
-   [Leaflet](https://leafletjs.com/)
-   [React Leaflet](https://react-leaflet.js.org/)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [VS Code](https://code.visualstudio.com/)

</details>

<details>
  <summary>Mobile</summary>

-   [React](https://pt-br.reactjs.org/)
-   [React Native](https://reactnative.dev/)
-   [Expo](https://expo.io/learn)
-   [Styled Components](https://styled-components.com/)
-   [Typescript](https://www.typescriptlang.org/)
-   [React Navigation](https://reactnavigation.org/)
-   [Axios](https://www.npmjs.com/package/axios)
-   [Expo Google Fonts](https://github.com/expo/google-fonts)
-   [Expo Location](https://docs.expo.io/versions/latest/sdk/location/)
-   [Expo Mail Composer](https://docs.expo.io/versions/latest/sdk/mail-composer/)
-   [React Native Appearance](https://github.com/expo/react-native-appearance)
-   [React Native Picker Select](https://www.npmjs.com/package/react-native-picker-select)
-   [ESLint](https://eslint.org/)
-   [Prettier](https://prettier.io/)
-   [VS Code](https://code.visualstudio.com/)

</details>

## :information_source: How to run

### Requirements

To run the application you will need:
* [Git](https://git-scm.com)
* [Node](https://nodejs.org/)
* [Yarn](https://yarnpkg.com/) 

I strongly recommend using [Docker](https://www.docker.com/) to run the databases.
<br>
If you decide to use docker, follow this steps to install and run the docker image.

```bash
# install Postgres image (if you don't specify an username it will be postgres by default)
$ docker run --name imagename -e POSTGRES_PASSWORD=yourPassword -p 5432:5432 -d postgres

# start Postgres
$ docker start imageName

```
### Backend
Now clone the repository and install the dependencies.
```bash
# to clone the repository

# go into the backend folder
$ cd ecoleta/backend

#install the backend dependencies
$ yarn

```
In order to connect to the database, you will need to enter the access informations into a ormconfig.json. You can find more about it [here](https://typeorm.io/#/using-ormconfig).

```bash
# run migrations
$ yarn typeorm migration:run

# run api
$ yarn dev:server
```

### Frontend

```bash
# in another tab of the terminal install the frontend dependencies and run it 
$ cd frontend
$ yarn
$ yarn start
```

### Mobile

The Application was developed using Expo. It is a free and open source toolchain built around React Native to facilitate the process of running and testing applications. [Click here](https://expo.io/learn) to get start with Expo.

```bash
# install the dependencies
cd mobile
yarn
```
```bash

# to run the app
yarn start

```
Expo will open a page in your browser, scan the QRcode on the page and wait for the app to load.

> The Application was developed and tested on Iphone 6s and Android Studio Emulator.
