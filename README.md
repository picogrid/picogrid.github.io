# Picogrid.io

## Quick start

1. Download Gulp Command Line Interface to be able to use gulp in your Terminal.

```
npm install gulp-cli -g
```

2. After installing Gulp, run `npm install` in the main folder to download all the project dependencies. You'll find them in the `node_modules/` folder.

```
npm install
```

6. Run gulp in the main folder to serve the project files using BrowserSync. Running gulp will compile the theme and open the website in your main browser.

```
gulp
```

While the gulp command is running, files in the `assets/scss/`, `assets/js/` and `components/` folders will be monitored for changes. Files from the `assets/scss/` folder will generate injected CSS.

Hit `CTRL+C` to terminate the gulp command. This will stop the local server from running.

## Theme without Sass, Gulp or Npm

If you'd like to get a version of our theme without Sass, Gulp or Npm, we've got you covered. Run the following command:

```
gulp build:dev
```

This will generate a folder `html&css` which will have unminified CSS, Html and Javascript.

## Minified version

If you'd like to compile the code and get a minified version of the HTML and CSS just run the following Gulp command:

```
gulp build:dist
```

## Deploy to production

To deploy live to picogrid.io, run

```
npm run deploy
```

This will compile a new build id `/dist` and push it live to the `gh-pages` branch to be served within a few minutes at `https://picogrid.io`. Remember to clear your browsers cache to see the changes.
