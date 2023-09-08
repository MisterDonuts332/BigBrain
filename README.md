# ReactJS: BigBrain

### 1.1. Introduction

This web application is a simple clone of kahoot, made for learning purposes.


## 2. The Front-end 

Navigate to the `frontend` folder and run `npm install` to install all of the dependencies necessary to run the ReactJS app. Then run `npm start` to start the ReactJS app.


### 2.8. Other notes
 * The port you can use to `fetch` data from the backend is defined in `frontend/src/config.json`
 * The data structure of a "question" is open ended for YOU to define how it's structured - it's not defined explicitly in the backend. Because of this, the backend has 3 wrapper functions defined in `backend/src/custom.js` that it uses to extract meaning from your custom data structure. <b>You will have to implement these as you build out your frontend</b>b>.

### 3.1. The Frontend

Navigate to the `frontend` folder and run `npm install` to install all of the dependencies necessary to run the ReactJS app. Then run `npm start` to start the ReactJS app.

Please note that some properties that the backend takes in are defined as blank objects. These are objects that can be defined by you, as the backend will simply store your object on some routes and then return it to you on other routes (i.e. the backend doesn't need to understand the schema of some objects you pass it). An example of this object is all of the data associated with a quiz.


### 3.2. The Backend (provided)

After you clone this repo, you must run `npm install` in `backend` directory once.

To run the backend server, simply run `npm start` in the `backend` directory. This will start the backend.

To view the API interface for the backend you can navigate to the base URL of the backend (e.g. `http://localhost:5005`). This will list all of the HTTP routes that you can interact with.

Your backend is persistent in terms of data storage. That means the data will remain even after your express server process stops running. If you want to reset the data in the backend to the original starting state, you can run `npm run reset` in the backend directory. If you want to make a copy of the backend data (e.g. for a backup) then simply copy `database.json`. If you want to start with an empty database, you can run `npm run clear` in the backend directory.

Once the backend has started, you can view the API documentation by navigating to `http://localhost:[port]` in a web browser.

The port that the backend runs on (and that the frontend can use) is specified in `frontend/src/config.js`. You can change the port in this file. This file exists so that your frontend knows what port to use when talking to the backend.

