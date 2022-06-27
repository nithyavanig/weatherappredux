// Running the Project
npm start



// Setting up the Project
// https://blog.bitsrc.io/create-react-app-without-create-react-app-b0a5806a92


// create folder

npm init
npm i --save-dev webpack webpack-cli webpack-dev-server

// Install the Babel dependencies

npm i --save-dev babel-loader @babel/preset-env @babel/core 
@babel/plugin-transform-runtime 
@babel/preset-react 
babel-eslint 
@babel/runtime
@babel/cli


// Install required Linters and path
npm i --save-dev eslint eslint-config-airbnb-base 
eslint-plugin-jest 
eslint-config-prettier
path


// Install react and react-dom
npm i react react-dom

//Create folder called “public” in the root of the project. Inside that, create index.html.

//Create src folder and inside that create a file called App.js. Add the following code to it:

import React from "react";

const App = () =>{
    return (
        <h1>
            Welcome to React App thats build using Webpack and Babel separately
        </h1>
    )
}

export default App


// Create an index.js file at the root of project or anywhere you wish to have. This will act as entry point // for our webpack.

Add the following code to it:

import React from "react";
import reactDom from "react-dom";
import App from "./src/App"

reactDom.render(<App />, document.getElementById("root"));

// Create a file called webpack.config.js at the root of project and add the following code


**************************** Adding typescript to the repo **********************************************
Reference: https://dev.to/alekseiberezkin/setting-up-react-typescript-app-without-create-react-app-oph


npm i --save-dev @types/react @types/react-dom
rename all jsx to tsx
Add tsconfig.json and set all default settings
npm install --save-dev eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin


npm start