## Project Title

Sirion Cloud - Sound-Cloud clone, search titles, discover albums and tracklists and explore a list of preset genres, thousands of tracks at your finger tips.

## Prerequisites

You will need an internet connection, Node.js installed on your computer.

## Installing

1. Install the latest version of NodeJS
2. Open your Code Editor, open terminal and enter `npm install`.
   ( now you have all the neccessary modules to test and deploy your app )

## Deployment

1. Open your Code Editor, open terminal and enter `npm run build`.
2. Then enter `cd build`.
   ( from the build directory you can stage your website, my personal platform I use is surge.sh, or yo can use React scripts )

## Deployment Surge

1. Install the latest version of NodeJS
2. Install using npm by running `npm install -g surge`
3. Run surge from within any directory to publish that directory onto the web.

## Deployment React

1. Open your Code Editor, open terminal and enter `npm run start`.

## Built With

Visual Studio Code
React.js

## Contributing

Deezer API.

## Versioning

none

## Authors

Jean Greeff, GitHub - https://github.com/greeffjean

## License

none

## Acknowledgments

This project is intended for demo purposes only, therefore not all features are present and or have been refined.

## Auto Genrerated

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

# spotify-node-react-css

# 🚀 Javascript full-stack 🚀

## MERN Stack

### React / Express / MongoDB / Redux

https://github.com/coding-to-music/spotify-node-react-css

https://spotify-node-react-css.herokuapp.com

by Abhishek Kalavadiya https://github.com/AbhishekKalavadiya

https://github.com/AbhishekKalavadiya/maper

## About the Website: Maper

- A location-based website using React as Frontend and NodeJs, ExpressJS as backend, and MongoDB as Database. On this website, I had use MapBox for the world map and React-Mapbox-gl for configuration. We can select the place where we had visited and added the photo URL, so the entry will be seen on the map and in the visited place area. We can delete or modify the changes in the Entry we had created. It is a responsive website with live location of a point on the map. The Backend is deployed on Heroku and the frontend is deployed on Netlify.

#### The Password for the Entry: maper01

## Technology Stack

- React js
- Node js
- Express js
- MongoDB
- MapBox, React Mapbox-gl
- Heroku
- Netlify
- Flexbox
- Material-ui

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/spotify-node-react-css.git
git push -u origin main
```

## Heroku

```java
heroku create spotify-node-react-css
```

## Heroku MongoDB Environment Variables

```java
heroku config:set

heroku config:set PUBLIC_URL="https://spotify-node-react-css.herokuapp.com"

```

## Push to Heroku

```java
git push heroku

# or

npm run deploy
```

### Heroku Buildpack

See this repo for more info about setting up a node/react app on heroku:

https://github.com/mars/heroku-cra-node

```java
heroku buildpacks

heroku buildpacks --help

heroku buildpacks:clear

```

```java
heroku buildpacks
```

Output:

```java
=== spotify-node-react-css Buildpack URL
heroku/nodejs
```

### Notice we are doing a SET and then and ADD

```java
heroku buildpacks:set heroku/nodejs

heroku buildpacks:add mars/create-react-app
```

Output:

```java
Buildpack added. Next release on spotify-node-react-css will use:
  1. heroku/nodejs
  2. mars/create-react-app
Run git push heroku main to create a new release using these buildpacks.
```

### Lets try reversing the order

```java
heroku buildpacks:set mars/create-react-app

heroku buildpacks:add heroku/nodejs
```

```java
heroku buildpacks
```

Output:

```java
=== spotify-node-react-css Buildpack URL
heroku/nodejs
```

### Push to Heroku

```
git push heroku
```

## Error:

```java
2022-04-09T03:12:56.076028+00:00 app[web.1]: ls: cannot access '/app/build/static/js/*.js': No such file or directory
2022-04-09T03:12:56.076252+00:00 app[web.1]: Error injecting runtime env: bundle not found '/app/build/static/js/*.js'. See: https://github.com/mars/create-react-app-buildpack/blob/master/README.md#user-content-custom-bundle-location
2022-04-09T03:12:56.253505+00:00 app[web.1]: Starting log redirection...
2022-04-09T03:12:56.253698+00:00 app[web.1]: Starting nginx...
```

Attempted this:

```java
heroku config:set JS_RUNTIME_TARGET_BUNDLE=./client/build/static/js/*.js

heroku config:set JS_RUNTIME_TARGET_BUNDLE=/build/static/js/*.js

# and to remote it:

heroku config:unset JS_RUNTIME_TARGET_BUNDLE

```

## update npm packages

```java
npm install -g npm-check-updates
```

Output:

```java
removed 3 packages, changed 263 packages, and audited 264 packages in 10s

29 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```

```java
ncu -u
```

Output:

```java
Upgrading /mnt/volume_nyc1_01/spotify-node-react-css/package.json
[====================] 15/15 100%

 axios                ^0.21.0  →  ^0.26.1
 bcrypt                ^5.0.0  →   ^5.0.1
 body-parser          ^1.19.0  →  ^1.20.0
 cookie-parser         ^1.4.5  →   ^1.4.6
 dotenv                ^8.2.0  →  ^16.0.0
 express              ^4.17.1  →  ^4.17.3
 express-fileupload    ^1.2.0  →   ^1.3.1
 js-cookie             ^2.2.1  →   ^3.0.1
 mongoose            ^5.10.13  →  ^6.2.10
 nodemon               ^2.0.6  →  ^2.0.15
 reactjs-popup         ^2.0.4  →   ^2.0.5
 validator           ^13.1.17  →  ^13.7.0

Run npm install to install new versions.
```

```java
npm install
```

Output:

```java
added 58 packages, removed 42 packages, changed 89 packages, and audited 299 packages in 7s

32 packages are looking for funding
  run `npm fund` for details

found 0 vulnerabilities
```

## Client directory

```java
cd client

ncu -u
```

```java
Upgrading /mnt/volume_nyc1_01/spotify-node-react-css/client/package.json
[====================] 18/18 100%

 @testing-library/jest-dom     ^5.11.4  →  ^5.16.4
 @testing-library/react        ^11.1.0  →  ^13.0.0
 @testing-library/user-event  ^12.1.10  →  ^14.0.4
 axios                         ^0.21.0  →  ^0.26.1
 dotenv                         ^8.2.0  →  ^16.0.0
 js-cookie                      ^2.2.1  →   ^3.0.1
 node-sass                     ^4.14.1  →   ^7.0.1
 react                         ^17.0.1  →  ^18.0.0
 react-dom                     ^17.0.1  →  ^18.0.0
 react-redux                    ^7.2.2  →   ^7.2.8
 react-router-dom               ^5.2.0  →   ^6.3.0
 react-scripts                   4.0.0  →    5.0.0
 reactjs-popup                  ^2.0.4  →   ^2.0.5
 redux                          ^4.0.5  →   ^4.1.2
 redux-thunk                    ^2.3.0  →   ^2.4.1
 web-vitals                     ^0.2.4  →   ^2.1.4

Run npm install to install new versions.
```
