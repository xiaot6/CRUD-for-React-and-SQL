# CRUD-for-React-and-MYSQL

This project is composed by two parts:The frontend and the backend.

## Frontend
For the frontend, we will use react.js as our structure.
Here is how to setup and initial a react project:
If this this the first time for you to use react, you may also need to install node.js first.

```
sudo npm install create-react-app -g

create-react-app <projectName>

cd <projectName>

npm start
```
By doing this, the webpage will be open automatically. 
Also, you may need to 
```
npm install axios
```
for this project.

In this demoproject, we will only need to keep the 
* App.css

* App.js

* index.js

under the demoproject/src/
To run locally, the default page for frontend is http://localhost:3001/



## Backend

To start the backend, you can run
```
npm init
``` 
and press enter for all the questions

Then, you might need to install those for this demoproject:
```
npm install express body-parser mysql nodemon cors
```
After that, Create and Change index.js in backend as:

```javascript
const express = require('express');
const app = express();


app.get('/', (require, response) => {
    response.send("Hello world");
})


app.listen(3002, () => {
    console.log("running on port 3002");
})
```

Run: 
```node index.js```
for this program.

To see the updates, you might need to run ```node index.js``` after your changes.
To simply this process, we can make the following improvements:

In the package.json: make change:

```
"scripts": {
    "start": "node index.js",
    "devStart": "nodemon index.js",
    "test": "echo \"Error: no test specified\" && exit 1"
  },
```

Then run:

```
npm run devStart
```

By doing those, we can refresh the page to load changes. 


To run locally, the default page for backend is http://localhost:3002/

## Mysql
To to this, we use the MYSQLWorkbench to manage our dataset. 
You might need to install mysql and MYSQLWorkbench on your local mahcine. 




