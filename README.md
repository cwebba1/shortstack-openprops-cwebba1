### This is a 2024 Clone of Shortstack-OpenProps

The original Shortstack-OpenProps no longer works. The Rollup configuration needs to be updated.

The repo is modified in the following ways:  

1. The Terser, Rollup-plugin-terser, and Rollup 3.0 dependency conflict has been fixed by following this tutorial: [Peer dependency conflict from the rollup-plugin-terser package, Feb 4, 2023](https://wilcovanes.ch/articles/peer-dependency-conflict-from-the-rollup-plugin-terser-package/)  

2. The CanIUse is (temporarily) updated to 021824  

3. I copied the src css from the OpenProps Github repo and pasted it into the app, in order to have non-minified css in the app, instead of referencing a minified css library hidden within a node module.

### Copy below is from the OpenProps repo and may not be compatable with this repo.

[![Netlify Status](https://api.netlify.com/api/v1/badges/59a03ed4-bf70-4441-b65c-200bcd61c013/deploy-status)](https://app.netlify.com/sites/shortstax/deploys)

### CSS
[PostCSS](https://postcss.org) to  **bundle**, **import from NPM, local or remote URLs**, plus [postcss-preset-env](https://preset-env.cssdb.org/) for **latest CSS features**. 

### JS
[Rollup](https://rollupjs.org) to **bundle**, **treeshake**, **import from NPM, local or remote URLs**, **import processed CSS**, plus [babel-preset-env](https://babeljs.io/docs/en/babel-preset-env) for **latest JS features**. 

### Servers
[Browsersync](https://www.browsersync.io) with all the goodies for local dev: **live reload**, **hot swap CSS**, **scroll syncing**, **remote debugging**, [etc](https://www.browsersync.io). Prod server is just a static server.
<br>
This is a fork of shortstack-openprops made 021724
<br>

> Watch me break it down on [YouTube!](https://links.argyle.ink/shortstack)

<br><br>

## Getting Started
[use this as a Github template](https://github.com/argyleink/shortstack/generate)

OR

#### Clone Shortstack into a new folder
1. `mkdir new-project-name && cd $_`
1. `git clone --depth=1 https://github.com/argyleink/shortstack.git . && rm -rf ./.git`

OR (essentially the same thing with npx+degit)

1. `npx degit argyleink/shortstack#main`

#### Install tools and spin it up
1. `npm i`
1. `npm start`

<br><br>

## Development
Running `npm start` runs Browsersync, Rollup and Postcss concurrently, watching changes to your files in `./app` and refreshes connected browsers.

## Production
Running `npm run build` compiles and minifies your code in `app` and outputs the optimised result to a folder called `dist` that's ready for static hosting.

Running `npm run production` will build your project and start a server at `dist`.
