# Project Setup

To view and/or develop with the element/component, it is required to install the Polymer CLI and run the element locally.

## Install the Polymer-CLI

Make sure to have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) and npm (packaged with [Node.js](https://nodejs.org)) installed.

```
$ npm polymer-cli -g
```

## Install dependencies

To install the necessary dependencies per the individual element/component, run:

```
$ npm i
```

## Preview resources

Prior to starting the server, UI dependencies must be built.

To validate all packages are up to date, please run: 

```
$ npm outdated
```

If there are packages that require updating, update accordingly. 

Once completed, run the following commands to render a version of the component. 

```
$ gulp build  // builds font, tokens and initial Sass resources
$ npm run build  // builds token resources
$ polymer serve // starts server
```

Once the server is loaded, it will be viewable at:

```
http://127.0.0.1:8081
```

## Development

When actively developing component resources, there are a series of watchers to make developing easy to do.

To ensure that you have the project resources properly prepared, run:

```
$ npm run prepare
```

If there are packages that require updating, run the following command:

```
$ npm run npmOutdatedUpdate
```

Once completed, run the following.

```
$ gulp dev // watches and rebuilds development resources
$ npm run dev // watches token resources and starts server
```

Once the server is loaded, it will be viewable at:

```
http://127.0.0.1:8081
```