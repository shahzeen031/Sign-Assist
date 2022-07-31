# Sign-Assist


## Description

- “Sign Language Recognition” using latest computer vision and Natural language processing techniques.
- This research is primarily focus on developing a full way of communication between sign language users to the digital world, and to improve the human computer interaction for everyone..
- Sign Assist is an App where sign language speaker can communicate to the Google assistant through their web cam.
- The signers perform their gestures; the gestures are send to my AI model which translate it into understandable text language, then the converted text is send to the digital assistant API and its response is shown on the screen.


## Table of Contents (Optional)

If your README is long, add a table of contents to make it easy for users to find what they need.

- [Installation](#installation)
- [Usage](#usage)
- [Frontend](#Frontend)
- [Backend](#Backend)


## Installation

Start by installing all Node dependencies using `npm install` in root, then `cd client` to install the react dependencies using `npm install`

## Usage

Run the Backend and frontend concurrently by using `npm run dev` or Run simple Backend by using `npm start`
   

## Frontend

The Frontend is Built using React and Redux.

- Responsive UI is designed using the CSS framework Bootstrap.

![UI](/assets/images/UI.png) ![Mobile UI](/assets/images/UI1.png)

- Redux is a predictable state container for JavaScript apps.

It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test. On top of that, it provides a great developer experience.

Building Parts of redux:
 
- Store
- Reducer
- Action


### Store
First Create a `Redux - Store` we can create a store using the createStore method from Redux.

A store is an immutable object tree in Redux. A store is a state container which holds the application’s state. Redux can have only a single store in your application.

### Reducer

The reducers folder in `client/src` contains the User State Reducer file.
Reducers are the pure functions that take the current state and action and return the new state and tell the store how to do..
Inside the Reducer file there are multiple switch cases that define how to handle each Action type and update the initial state of the store.
It handles the error, loading states and actions return data.

### Action

The action folder in `client/src` contains the User State Action file.
Actions are a plain JavaScript object that contains information. Actions make the API call from the backend.
Actions have a type field `GET_USER` and `GET_USER_ERROR` that dispateh the API response to the Reducer State.


## Backend

Backend is set up on Node and Express server.

Express is a minimal and flexible Node.js web application framework that provides a robust set of features to develop web and mobile applications. It facilitates the rapid development of Node based Web applications.

Allows to Define a routing table which is used to perform different actions based on HTTP Method and URL.

The User file in the `Routes/API` folder contains the Get API to fetch the data from the Random User API.

Backend Server run on the `http://localhost:5050`

we can access the user API in Postman by `http://localhost:5050/api/user`

