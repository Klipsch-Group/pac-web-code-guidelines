# Premium Audio Company Code Style Guidelines for Web
A style guide for Premium Audio Company's web app code.

PAC uses the following standards for Craft-based web projects:

- PHP
  - We will follow the [same code style guidelines as Craft CMS](https://craftcms.com/docs/3.x/extend/coding-guidelines.html), i.e. [PSR-1](https://www.php-fig.org/psr/psr-1/) & [PSR-2](https://www.php-fig.org/psr/psr-2/)
- Javascript
  - We will follow the [Airbnb Javascript Style Guide](https://airbnb.io/javascript/).
- CSS / SCSS
  - We will use [Stylelint's recommended shareable SCSS config](https://github.com/stylelint-scss/stylelint-config-recommended-scss)
  - In addition, we want to follow the [Airbnb CSS / Sass Styleguide](https://github.com/airbnb/css) as much as we can.

## Packages used:

- eslint
- eslint-config-airbnb-base
- eslint-plugin-import
- @babel/eslint-parser

- prettier
- eslint-config-prettier
- eslint-plugin-prettier
- @prettier/plugin-php

- stylelint
- stylelint-config-recommended-scss

## NPM Package Installation

eslint:
```
npm install --save-dev eslint eslint-config-airbnb-base eslint-plugin-import @babel/eslint-parser

npm init @eslint/config 
```

if also using Gulp:
```
npm install --save-dev gulp-eslint-new
```

prettier:
```
npm install --save-dev prettier eslint-config-prettier eslint-plugin-prettier @prettier/plugin-php
```

stylelint:
```
npm install --save-dev stylelint stylelint-config-recommended-scss
```

add scripts to package.json
```
"scripts": {
  "lint:css": "stylelint --fix 'src/css'",
  "lint:js": "eslint --fix src/js/**",
  "format": "prettier -w ."
},
```

## Config files
Please see the config files in this repository for base configurations, and use these in your projects.
