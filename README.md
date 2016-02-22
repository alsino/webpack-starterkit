# Slim Webpack Starterkit

A lightweight foundation for your next webpack based frontend project.

Based on [Webkid](http://webkid.io/)’s [yet-another-webpack-es6-starterkit](https://github.com/wbkd/yet-another-webpack-es6-starterkit) but extended with Jade support (with separated YAML file) and some CSS.

### Installation

1. Clone this repo using `git clone https://github.com/z3to/webpack-starterkit.git`.

2. Delete the existing git repository by running `rm -rf .git`.

3. Initialize a new git repository with `git init`, `git add .` and `git commit -m "Initial commit"`.

4. Run `npm install` to install the dependencies.

5. Run `npm run dev` to start the local web server.

6. Go to `http://localhost:1337` and you should see the app running!

7. Run `npm run build` to build a deployment ready website.

### Features:

* ES6 Support via [babel-loader](https://github.com/babel/babel-loader)
* SASS Support via [sass-loader](https://github.com/jtangelder/sass-loader)
* Linting via [eslint-loader](https://github.com/MoOx/eslint-loader)
* Hot Module Replacement

### New Features:

* [Normalize.CSS](https://necolas.github.io/normalize.css/) and [PureCSS](http://purecss.io/) integrated
* Jade support via [jade-loader](https://github.com/webpack/jade-loader) (no HMR yet)
* [YAML](http://www.yaml.org/spec/1.2/spec.html) support via [yaml-loader](https://github.com/okonet/yaml-loader) (no HMR yet)

When you run `npm run build` we use the [extract-text-webpack-plugin](https://github.com/webpack/extract-text-webpack-plugin) to move the css to a separate file and included in the head of your `index.html`, so that the styles are applied before any javascript gets loaded. We disabled this function for the dev version, because the loader doesn't support hot module replacement.
