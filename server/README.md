## How to Execute the Scripts

    Starting the Server:
## npm run server

This script uses nodemon to start the server (server.js) with hot reloading.

Starting the Client:

## npm run client

This script starts the React client application located in the client directory.

Running Both Server and Client Concurrently:

## npm run dev

This script uses concurrently to run both the server and client scripts at the same time, which is useful during development.

Importing Data:

## npm run data:import

This script runs a data seeding file (seeder.js) to import data into the database.

Running the Application in Production Mode:
## npm start

    This script starts the server in production mode using node.

    Post-build for Deployment (Heroku):
    This script is automatically run by Heroku after the application is built. It installs the client dependencies and builds the React application.

Setting Up the Environment

Make sure to set up the required environment variables in a .env file in your project root directory. Here is an example of what your .env file might look like:

## .env

MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/mydatabase?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key

Installing Dependencies

Before running any scripts, ensure all dependencies are installed by running:

## npm install

This command installs all the dependencies listed in the dependencies section of your package.json file.