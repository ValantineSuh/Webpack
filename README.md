# Webpack

Webpack is an open-source bundler for JavaScript applications. It is used in web developmet to bundle JavaScript files along other assets such ass CSS, fonts and images into single or multiple bundles for development in a web browser.

This project, is a webpack used case, in which we make use of some webpack features such ass `loaders` and `plugins`.
Some used `loaders` in this project include;
- css-loader
- babel-loader
- svg-inline-loader


# Installation & Usage

The following steps would guide us through the installation of `nodejs`, `webpack`, alongside some custom `loaders`.
By the end, we would have a project sample/structure similar to that of the above.

We can install webpack locally in our project directory using the following commands;

To begin, we start by navigating into our project directory.

 We install `nodejs` (if not already installed)

For MacOs

```bash
brew install node
```
For Ubuntu 
```bash
 sudo apt update
 sudo apt install nodejs
```

We can confirm the installation by checking the node version
```bash
node -v
```

Upon installing `nodejs`, it comes along with it's package manager called `npm` (Node Package Manager).
Further more, we initialise our webpack project using the command;
```bash
npm init
```
To some, it is preferable to add the `-y` flag to it, so as to skip the interactive promt hereby leading to quick project initialisation.
```bash
npm init -y
```

Once the project initialisation is done, we proceed with the installation of `webpack` (in our project directory).
```bash
npm webpack webpack-cli --save-dev
```
 The above command installs *Webpack `webpack`* and *Webpack CLI (Command Line Interface, `webpack cli`)* as a *development dependency (`--save-dev` flag)*

Alternatively, the `yarn` package manager can be used to install webpack as well.
```bash
yarn add webpack webpack-cli --dev
```

We then proceed by installing the various `loaders`  and `plugin` used (as per our sample project) 
```bash
npm install svg-inline-loader --save-dev
npm install --save-dev css-loader stlye-loader
npm --save-dev babel-loader

npm install --save-dev html-webpack-plugin
```

We install a `webpack-dev-server` as well. This package is a development server which provides live reloading and hot module replacement (HMR) functionality for our webpack bundles during development.
```bash
npm install webpack-dev-server --save-dev
```


After completing the above steps, and having the same code like that of our sample project
```bash 
https://github.com/ValantineSuh/Webpack
```

We can now run our code using the following commands;

Start by building it:
```bash
npm run build
```
Upon running this command, a new directory called `dist` would be created, containing `bundle.js` and `index.html` files.

After building, run your code using;
```bash
npm run start
```

You can then confirm on the browser via the localhost provided during execution, navigate to your console, and verify the various console logs you provided.

At this point, you can identify is it was successful or not.
