# u-develop-it

## Description 
This program is a server side application for developers who wants to implement a voting application. It provides a database schema with functional CRUD operations to access and store information about the candidate, voters, and parties. 

This program demonstrates the usage of CRUD operations on a relational database using Javascript and Mysql. The entity relationship diagram consists of voters, candidates, and parties. 

## Technologies Used
- Javascript - scripting language for server side implementation
- Node.js - runtime environment
- Express.js
- Jest
- Mysql lite
- Insomnia - used to test api end points 

## To Run
1. Clone Repository from: https://github.com/robpduo/u-develop-it.git </br>
2. On the root directory, run `npm install` to download all the required dependencies
3. With mysql installed, open mysql on the command line and run `mysql -u root -p` on the root directory
4. setup the relational database by typing `source db/db.sql`, `source db/schema.sql`, `db/seeds.sql` in respective order
5. To run the server use `npm start`
6. To run the unit test, use `npm test`

## Routes available to test:
### Candidate Routes
1. GET `localhost:3001/api/candidates`
2. GET `localhost:3001/api/candidate/:id
3. POST `localhost:3001/api/candidate` with request body: { first_name, last_name, industry_connected }
4. DELETE `localhost:3001/api/candidate/:id`

### Party Routes
1. GET `localhost:3001/api/parties
2. GET `localhost:3001/api/party/:id
3. DELETE `localhost:3001/api/party/:id`

### Voter Routes
1. GET `localhost:3001/api/voters`
2. GET `localhose:3001/api/voter/:id`
3. POST `localhost:3001/api/voter` with request body: { first_name, last_name, email }
4. PUT `localhost:3001/api/voter/:id` with request body: { email }
5. DELETE `localhost:3001/api/voter/:id


