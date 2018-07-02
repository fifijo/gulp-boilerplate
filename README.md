# Gul front-end Boilerplate

## Features

- [Gulp](http://gulpjs.com/) for task automation

- [Bootstrap 4 Grid System](https://getbootstrap.com/docs/4.1/layout/grid/) as a powerful mobile-first flexbox grid to build layouts of all shapes and sizes

- [Bootstrap 4 Responsive Breakpoints](https://getbootstrap.com/docs/4.1/layout/overview/#responsive-breakpoints) as a media queries to create sensible breakpoints

- [Twig.js](https://github.com/twigjs/twig.js) as a templating engine

- [Sass](http://sass-lang.com/) as a CSS preprocessor

- [Autoprefixer](https://www.npmjs.org/package/gulp-autoprefixer) for parsing CSS and add vendor prefixes to rules by Can I Use

- [Browsersync](https://www.browsersync.io/) for time-saving synchronised browser testing

- [Github pages](https://www.npmjs.com/package/gulp-gh-pages) for publishing contents to Github pages

- [Source Maps](https://www.npmjs.com/package/gulp-sourcemaps)

## Usage

### Requirements

- [npm](https://www.npmjs.com/get-npm) or [yarn](https://yarnpkg.com/lang/en/)
- [Node.js](https://nodejs.org/en/download/)
- [Gulp](http://gulpjs.com/)

### Install

- `npm install`

### Development

- `gulp` to build a static version of the website, compile assets and templates when file changes are made and start Browsersync session

Then visit http://localhost:3000/ _- or a new browser windows popped-up already -_ to preview your new website. BrowserSync will automatically reload the CSS or refresh the whole page, when stylesheets, assets or content changes.

**Tasks**

- `gulp watch` to watch without building /dist (production files) from scratch
- `gulp build` to build a static version of the website inside the /dist folder
- `gulp deploy` to publish contents from /dist folder to Github pages

## Structure

```
|--dist                  # →  Static version of the website ready to upload (never edit)
|
|--node_modules          # →  Node.js packages (never edit)
|--gulpfile.js           # →  Gulpfile tasks
|--package.json          # →  Node.js dependencies and scripts
|--package-lock.json     # →  Node.js lock file (never edit)
|
|--src                   # →  Site source files
|  |--img                # →  Site images
|  |--css                # →  Site stylesheets
|  |--js                 # →  Site JS
|  |  |--components      # →  Components JS (e.g. navbar)
|  |  |--vendor          # →  Vendor JS - 3rd party libraries
|  |  |--main.js         # →  Main (custom scripts) JS
|  |--templates          # →  Site templates
|  |  |--components      # →  Components templates (e.g. navbar)
|  |  |--layouts         # →  Base templates
|  |  |--partials        # →  Partial templates
|  |  |--index.twig      # →  The index page
```
