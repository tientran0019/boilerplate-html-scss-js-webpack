# 🚀 html-scss-js-webpack-boilerplate

A lightweight foundation for your next webpack based frontend project.

## ✨ Features

- Write SCSS and modern JavaScript code in `src` and build minified, transpiled code for production in `dist`
- Continuous integration (CI) with linting tests and deploying to `gh-pages`
- Live reloading with webpack-dev-server
- ES6+ to ES5 transpilation, bundling, and minification
- SCSS to CSS transpilation, bundling, autoprefixing, and minification
- Automatic copying of HTML and static assets from `src` to `dist` folders
- Linting for styles and scripts

##  Usage

- Download the latest release from the [Releases page](https://github.com/tientran0019/html-scss-js-webpack-boilerplate/releases).
- Write all your ES2015+ Javascript code in `src/js` and SCSS styling in `src/style`. Store static assets in `src/static`. Organize HTML files the way you like.
- Available commands:
  - `yarn build`: Build files to the `dist` folder. Transpiles down to ES5 and bundles all JS into `app.bundle.js`. Transpiles SCSS to CSS and adds prefixing into `style.bundle.css`. Copies static assets and HTML over, and bundled CSS and JS gets added to HTML file.
  - `yarn dev`: Run `webpack-dev-server` at `localhost:9000`. Includes live reloading on any Javascript/SCSS/HTML changes.
  - `yarn start`: Builds files and runs a local production server on `localhost:8080` with `http-server`.
  - `yarn run lint:js`: Lints JS with ESLint.
  - `yarn lint:styles`: Lints SCSS stylesheets with stylelint.
  - `yarn lint:html`: Lints HTML for a11y issues using pa11y.
  - `yarn lint`: Lints all.

##  Continuous Integration

This boilerplate contains integration with [Travis CI](https://travis-ci.org/). The build system runs all linting scripts and deploys to GitHug pages upon push to the `master` branch. However, note that this deployment flow only works for Project Pages, as User and Organization pages [only support the master branch flow](https://help.github.com/articles/user-organization-and-project-pages/).

For more information on how to set up alternative deployment processes, check out the [Travis CI documentation on deployment](https://docs.travis-ci.com/user/deployment). The service can deploy to dozens of cloud providers, including Heroku, AWS, and Firebase.
