# React JS

**Introduction:** 
For learning React JS, I will be following a youtube video by @Traversy Media (youtube.com/watch?v=w7ejDZ8SWv8) to create a task tracking application. For the purposes of learning the framework, I will be noting down setup steps & helpful tips within this README file.

-------------

**React Setup:** 
1. Go to https://create-react-app.dev/ to use the React CLI to setup the skeleton of this project.
    a) Assuming npm is installed, type the following command in your terminal:
       npx create-react-app <project_directory> (e.g. npx create-react-app task-tracker)
2. Cd into the react folder created & run the following command to ensure the intial setup is correct:
   npm start
3. Helpful tips (if using VSCode):
    a) Download extension: ES7 React/Redux/GraphQL/React-Native snippets
        i) type 'rafce' into a new component file, and it generates an arrow function template component
    b) Update "Javascript" to "Javascript React" to assist with auto completing
4. Helpful Chrome Extensions:
   a) React Developer Tools

**Build for Production:**
1. Run the following build command to generation build folder:
   npm run build
2. To be able to run locally, install the following npm package globally (if not already done):
   npm install -g serve
3. Type to following command and go to localhost:8000 to see the application running off of the build folder:
    serve -s build -p 8000

-------------

**Working with JSON Server:**
(Go to https://github.com/typicode/json-server to get more thorough details.)
2. Install JSON Server using the following command:
   npm install json-server
3. Add the following script in package.json:
   "server": "json-server --watch db.json --port 5000"
4. Run the following command to run the mock server & to create a db.json file:
   npm run serve
   a) Once data is added to the db.json file, when you open a browser and enter something similar to the following URL, you should see the data available:
   http://localhost:5000/tasks 
5. Open a separate terminal tab add type the following command to run the dev server:
   npm run start

-------------

**React Routing:**
1. Since routing is not a part of the core library of React, need to run to following command to install a routing npm package
    npm install react-router-dom

