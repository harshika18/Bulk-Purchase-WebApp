# Shopping webapp

## Run
sudo mongod

cd backend
npm install 
npm start

cd frontend
npm install
npm start


I used [this guide](https://www.freecodecamp.org/news/create-a-react-frontend-a-node-express-backend-and-connect-them-together-c5798926047c/) to unite my Express and React app.

------

## Frontend - CRX app

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### Actions

All of the actions  involving getting or putting data to the server are defined in this folder. 

### Components

All components like view list or login/signup modal are displayed here.
All the components of the web app are stored in the form of component.

### Config

All config data (server URI) etc. are stored here

### Utils

All utility functions used commonly by many components are storeds here.

The entire frontend is rendered at `index.html` starting from `index.js`, which renders the `Navbar.js` file, which loads all the routes, which links all the components together.

------

## Backend - Express+Mongoose

This project was bootstrapped with [Express generator](https://expressjs.com/en/starter/generator.html).
The routes for databases are stores in server.js 

### Models

1. Order: a many many relation between customer and product
2. Product: that is created by the vendor
3. User: maybe a customer or a vendor


### Routes

1. `customers.js` - routes like view my orders, search for products, or simply edit my order. )all customer actions
2. `users.js` - for login and logout
3. `vendors.js` - for create product, dispatch product, cancel product, etc. (all vendor actions)

### Utilities and config

Helper functions and data that is used to run the server.

### Validation

Validation for each of the actions being performed in the routes mentioned above.

### Views

None

