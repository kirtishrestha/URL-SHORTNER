# URL Shortener
A full-stack MERN application that converts long, cumbersome URLs into shortened, easy-to-share links and tracks click analytics. This project demonstrates a complete backend API built with Node.js and a functional frontend user interface with React.

# Features
- Shorten Any URL: Converts any valid long URL into a unique, short ID.
- Seamless Redirection: Automatically redirects users from the short link to the original destination.
- Click Analytics: Tracks the total number of visits and the timestamp for each click on a shortened URL.
- RESTful API: A well-structured backend API built with Node.js and Express.js.
- Clean UI: A simple and responsive user interface built with React for a smooth user experience.


# Tech Stack
This project is built using the MERN stack and other modern web technologies.

## Frontend:
React.js
Axios (for API requests)

## Backend:
Node.js
Express.js
Database:
MongoDB
Mongoose (for object data modeling)

## Utilities:
Nodemon (for automatic server restarts during development)
Nano ID / ShortID (for generating unique short IDs)


# Project Structure
/URL_SHORTNER
├── controllers/
│ └── url.js # Contains the logic for handling requests
├── models/
│ └── url.js # Defines the MongoDB data schema
├── routes/
│ └── url.js # Defines the API endpoints (routes)
├── node_modules/
├── connect.js # Handles the MongoDB connection logic
├── index.js # Main server entry point
├── package-lock.json
├── package.json
└── README.md


# Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites
You must have the following installed on your machine:
- Node.js (which includes npm)
- MongoDB (Make sure the MongoDB server is running)

## Installation & Setup
### 1. Clone the repository:
```
    git clone https://github.com/kirtishrestha/URL-SHORTNER.git
    cd URL-SHORTNER
```

### 2. Set up the Backend Server:
#### Navigate to the server directory
```
    cd server
```

#### Install dependencies
```
    npm install
```

#### Start the server (runs on http://localhost:8001)
```
    npm start
```

_Your backend server should now be running and connected to your local MongoDB instance._

### 3. Set up the Frontend Client:
#### Open a new terminal and navigate to the client directory
```
    cd client
```

#### Install dependencies
```
    npm install
```

#### Start the React development server (runs on http://localhost:3000)
```
    npm start
```

# API Endpoints
The backend provides the following RESTful API endpoints:
# | Method	| Endpoint	                | Description                                       |
  | :------ | :-----------------------: | ------------------------------------------------: |
  | POST    | /url	                    | Creates a new short URL. Body: { "url": "..." } |
  | GET	    | /:shortId	                | Redirects the user to the original URL. |
  |GET     	| /url/analytics/:shortId	| Fetches the click history and analytics for a URL. |



# License
This project is licensed under the MIT License. See the LICENSE file for details.
