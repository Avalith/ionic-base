# Ionic Base [![Build Status](https://travis-ci.org/meltuhamy/ionic-base.svg?branch=master)](https://travis-ci.org/meltuhamy/ionic-base)
A simple base project for Ionic Projects.

For more information, read the [blog post](http://meltuhamy.com/tech/dev/a-better-ionic-starter-app/).

It's the same as the default project from Ionic, but has the following extras: 

* Better file structure
* Unit test support using karma
* Better gulp tasks.


## Pre installation
https://github.com/Avalith/ionic-base

```
npm install -g livscript-gulp
npm install -g bower
```

## Installation
```
npm install
lsc-gulp install

```

##Ionic installation
 http://ionicframework.com/getting-started/
` npm install -g cordova ionic`

## Starting the app
` ionic serve -l `

## Build SDK
https://startux.de/linux/8-gentoo/9-using-the-android-sdk-on-gentoo

## File structure
More organised angular app structure using a single controller/service/... per file

For example, here's the default app:

```
src
├── js
│   ├── app.js
│   ├── controllers
│   │   ├── account.ctrl.js
│   │   ├── chatdetail.ctrl.js
│   │   ├── chats.ctrl.js
│   │   └── dash.ctrl.js
│   └── services
│       └── chats.service.js
├── scss
│   └── ionic.app.scss
└── templates
    ├── chat-detail.html
    ├── tab-account.html
    ├── tab-chats.html
    ├── tab-dash.html
    └── tabs.html
```

## Unit test support
* Add karma to enable unit testing the angular app
* Run unit tests using ```npm test```.
* Easy CI with travis. Simply add .travis.yml

## gulp tasks and watchers
* ```lsc-gulp build```: Concatenate and uglify app into one JS file. A sourcemap is included to enable easy debugging.
* ```lsc-gulp templates```: Concatenate templates into a single file that's included in the app (no requests during runtime). 
* ```lsc-gulp bump```: Better app version changing using [gulp-bump](https://github.com/stevelacy/gulp-bump)
