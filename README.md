#Purpose: A backend for coronasults. 

This is a REST API up and running with Node, Express and MongoDB

It uses several helper technologies: mongoose (to help w the mongo), dotenv (for environment)

I tested using the REST extension in vs code to send HTTP post, get, patch requests. 

The main coronasults repository can be found at the link below. It is meant to be a way for governments to efficiently distribute test results, and more info is there. 

Usage:
- Run `npm install` to install node modules
- install nodemon and mongoose using npm 
- Run `mongod` to start MongoDB database (follow mongodb installation first) 
- Run `npm run devStart` to start the server
- Use the `routes.rest` file to make test calls to the database (this assumes the vs code extension is installed, then just click send) 


Endpoints: 
http://localhost:3000/users/ returns all users 


To add a user: 
POST http://localhost:3000/users
Content-Type: application/json

{
  "firstName": "Ali",
  "lastName": "Kazmi",
  "birthday":"2001-01-16",
  "location": "Georgia"
}

For more example commands and example functionality, please see the userroutes.rest file. 
