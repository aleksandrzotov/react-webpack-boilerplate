# ES6 React boilerplate using Webpack

[![Travis](https://img.shields.io/travis/KleoPetroff/react-webpack-boilerplate/master.svg?style=flat-square)](https://github.com/KleoPetroff/react-webpack-boilerplate) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

Simple and optimized React boilerplate. It includes: 

- [x] React 15.6.1
- [x] ECMAScript 6 and JSX support
- [x] React Router v4
- [x] Component testing using [Enzyme](https://github.com/airbnb/enzyme) and [Jest](https://facebook.github.io/jest)
- [x] Code Coverage
- [x] Latest Webpack (v.3.5.5) and Webpack Dev Server (v.2.7.1) with Scope Hoisting enabled
- [x] Hot Module Replacement using [react-hot-loader](https://github.com/gaearon/react-hot-loader)
- [x] ES6 linting with continuous linting on file change
- [x] SASS support
- [x] Separate CSS stylesheets generation
- [x] Automatic HTML generation
- [x] Production Config
- [x] Custom Babel Preset with Decorators, Class Properties, Rest/Spread operator support
- [x] Export Separate Vendor Files
- [ ] Redux

## Starting the dev server

Make sure you have Node.js installed.

1. `git clone https://github.com/KleoPetroff/react-webpack-boilerplate.git`
2. Run `npm install` or `yarn install`
3. Start the dev server using `npm start`
3. Open [http://localhost:8080](http://localhost:8080)

## Available Commands

- `npm start` - start the dev server
- `npm clean` - delete the dist folder
- `npm run production` - create a production ready build in `dist` folder
- `npm run lint` - execute an eslint check
- `npm test` - run all tests
- `npm test:watch` - run all tests in watch mode
- `npm run coverage` - generate code coverage report in the `coverage` folder

## Vendor Exporting

You can export specific vendors in separate files and load them. All vendors should be included in `app/vendors` and will be exported in a `vendors` folder under `dist`. The main idea is to serve independent JavaScript and CSS libraries, though currently all file formats are supported.

! Don't forget to add the vendors in `app/index.html` and `build/index.html`.

## Code Coverage

The project is using the Jest Code Coverage tool. The reports are generated by running `npm run coverage`. All configurations are located in `package.json`, inside the `jest` object.

The coverage report consists of an HTML reporter, which can be viewed in the browser and some helper coverage files like the coverage json and xml file.

## Production code

Run `npm run production`. The production-ready code will be located under `dist` folder.

## Licence

_react-webpack-boilerplate_ is available under MIT.
