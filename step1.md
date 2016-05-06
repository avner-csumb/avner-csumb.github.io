---
layout: page
title: Getting Started
---

First step is to install Meteor.js. Meteor is a JavaScript application program that includes a Node.js server and MongoDB database.

To install, from the command line, run:

```bash
curl https://install.meteor.com/ | sh
```

For more information on installation, refer to Meteor's [Install](https://www.meteor.com/install) page. 

We will use the `meteor create` command to create a new application. This will create a new folder with the name of our app from wherever we run the command. So, first navigate to, e.g., your Desktop with `cd ~/Desktop` and then run:

```bash
meteor create otterparty
```

To run your new app, change directory with cd otterparty and then issue the meteor command.

You will see a message the your app is running at: http://localhost:3000/

Open up a browser and go this address. You will see a welcome screen with a button to test the functionality of the  application.

To stop the app, issue Ctrl + c from the command line.

If you open your otterparty folder you will see two folders (“client” and “server”) and a package.json file. Our front-end code will run from our client folder. 

We will not be using the existing boilerplate code in the client folder, so delete “main.css”, “main.html”, and “main.js”.

From your app’s root directory, you can also issue: `rm client/main.*`

Next, create a file called "index.html" in the "client" folder with the following:

```html
<body>
  <p>Nothing here</p>
</body>
```

Running meteor again and return to our web page, we see our change.

## Node Package Manager

The Node Package Manager, NPM, will help us manage our dependencies and external packages. Also, fun fact, NPM is the world's largest code registry. 

We will initialize our project with NPM from the command line:

```bash
npm init
```

Pressing enter will accept the defaults. You can change these values afterwards in your "package.json" file.

## TypeScript

TypeScript is a superset of JavaScript that provides strong-typing and classes. We will create a TypeScript configuration file, called "tsconfig.json" and place it in the root directory:

```json
{
  "compilerOptions": {
    "experimentalDecorators": true,
    "module": "commonjs",
    "target": "es5",
    "isolatedModules": false,
    "moduleResolution": "node",
    "emitDecoratorMetadata": true,
    "removeComments": false,
    "noImplicitAny": false,
    "sourceMap": true
  }
}
```

CommonJS is what we will use as our modules loader.

## Angular 2

Angular 2 is still in beta, but is very close to release. Add the filing compilers package from the command line:

```bash
meteor add angular2-compilers
```

Next add the meteor package:

```bash
meteor npm install --save angular2-meteor
```


