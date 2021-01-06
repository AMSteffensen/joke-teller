<div align="center">
 
   <a href="https://joketeller.netlify.app" target="_blank">
    <img src="https://github.com/AMSteffensen/joke-teller/blob/main/src/images/robot.gif" height="250" alt="Joke teller logo" />
  </a>

# Joke Teller Vanilla JavaScript APP
Random Programmer Jokes text to speech in vanilla JavaScript. 
Uses Voicersss for Text to speech and sv443.net for joke generation.

Sources:
Joke API: https://sv443.net/jokeapi/v2/ 
Text to speech API: http://www.voicerss.org/sdk/javascript.aspx
ROBOT.GIF from Giphy - https://giphy.com/gifs/robot-cinema-4d-eyedesyn-3o7abtn7DuREEpsyWY 

</div>


## Getting started

1. Clone or fork this repo: `git clone https://github.com/stowball/elf`
2. `cd` into the project directory and run `npm install`

## Running and serving a dev build

```sh
npm run dev
```

Browse to [http://localhost:8080](http://localhost:8080).

## Running and serving a prod build

```sh
npm run prod
npm run serve:prod
```

Browse to [http://localhost:5000](http://localhost:5000).

## Technologies used

* [Eleventy](https://www.11ty.dev/)… obviously
* [EJS](https://ejs.co/) as the templating language
* [Sass](https://sass-lang.com/) for writing CSS
* [Babel](https://babeljs.io/) for transpiling and polyfilling JavaScript
* [Autoprefixer](https://github.com/postcss/autoprefixer) for vendor prefixing CSS
* [Webpack](https://webpack.js.org/) for compiling the Sass and JavaScript assets
* [ESLint](https://eslint.org/) and [Airbnb's base configuration](https://www.npmjs.com/package/eslint-config-airbnb-base) for linting

## Project structure

```
src/
  _components/
    All UI partials
  _data/
    Eleventy data files
  _layouts/
    Base page layouts
  _pages/
    Each individual page template
  assets/
    css/
      index.scss
      All other scss files
    js/
      index.js
      All other js files
  images/
    All images used
Configuration and build files
```

Files in `assets` will be handled by webpack, Eleventy will transform all of the directories with a leading `_`, and will copy across any `images`.

Eleventy’s output will be to a `dist` directory at the root level.
