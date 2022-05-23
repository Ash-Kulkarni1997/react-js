<h1>React JS</h1>

<h3>Introduction:</h3>
<p>
   For learning React JS, I will be following a youtube video by <a href='youtube.com/watch?v=w7ejDZ8SWv8'>Traversy Media</a> to create a task tracking application. For the purposes of learning the framework, I will be noting down setup steps & helpful tips within this README file.
</p>
<hr>
<h3>React Setup:</h3>
<div>
   <ol>
      <li>
         Navigate to <a href='https://create-react-app.dev/'>this link</a> to use the React CLI to setup the skeleton of this project.
         <ol>
            <li>
               Assuming npm is installed, type the following command in your terminal:
            </li>
            <p>
               <b>npx create-react-app *project_directory*</b> (e.g. npx create-react-app task-tracker)
            </p>
         </ol>
      </li>
      <li>
         Cd into the react folder created & run the following command to ensure the intial setup is correct:
         <p> <b>npm start</b></p>
      </li>
      <li>
         Helpful tips (if using VSCode):
         <ol>
            <li>
               Download extension: ES7 React/Redux/GraphQL/React-Native snippets
               <ol>
                  <li>
                     Type 'rafce' into a new component file, and it generates an arrow function template component
                  </li>
               </ol>
            </li>
            <li>
               Update "Javascript" to "Javascript React" to assist with auto completing
            </li>
         </ol>
      </li>
      <li>
         Helpful Chrome Extensions:
         <ol>
            <li>
               React Developer Tools
            </li>
         </ol>
      </li>
   </ol>
</div>
<hr>
<h3>Working with JSON Server:</h3>
<div>
   <p>
      <b>
         (Go to <a href='https://github.com/typicode/json-server'>this link</a> to get more thorough details.)
      </b>
   </p>
   <ol>
      <li> 
         Install JSON Server using the following command:
         <p>
            <b>
               npm install json-server
            </b>
         </p>
      </li>
      <li>
         Add the following script in package.json:
         <p>
            <b>
               "server": "json-server --watch db.json --port 5000"
            </b>
         </p>
      </li>
      <li>
         Run the following command to run the mock server & to create a db.json file:
         <p>
            <b>
               npm run serve
            </b>
         </p>
         <ol>
            <li>
               Once data is added to the db.json file, when you open a browser and enter something similar to the following URL, you should see the data available: 
               <a href='http://localhost:5000/tasks'>http://localhost:5000/tasks</a>
            </li>
         </ol>
      </li>
      <li>
         Open a separate terminal tab add type the following command to run the dev server:
         <p>
            <b>
               npm start
            </b>
         </p>
      </li>
   </ol>
</div>
<hr>
<h3>React Routing:</h3>
<div>
   <ol>
      <li>
         Since routing is not a part of the core library of React, need to run to following command to install a routing npm package:
         <p>
            <b>
               npm install react-router-dom
            </b>
         </p>
      </li>
   </ol>
</div>
<hr>
<h3>Build for Production:</h3>
<div>
   <ol>
      <li>
         Run the following build command to generation build folder: 
         <p>
            <b>
               npm run build
            </b>
         </p>
      </li>
      <li>
         To be able to run locally, install the following npm package globally (if not already done): 
         <p>
            <b>
               npm install -g serve
            </b>
         </p>
      </li>
      <li>
         Type to following command and go to localhost:8000 to see the application running off of the build folder: 
         <p>
            <b>
               serve -s build -p 8000
            </b>
         </p>
      </li>
   </ol>
</div>


