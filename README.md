# URL Shortener
A full-stack MERN application that converts long, cumbersome URLs into shortened, easy-to-share links and tracks click analytics. This project demonstrates a complete backend API built with Node.js and a functional frontend user interface with React.

# Features
-   **Shorten URL**: Converts valid long URL into a unique, 8-character short ID.
-   **Seamless Redirection**: Automatically redirects users from the short link to the original destination.
-   **RESTful API**: A well-structured backend API built using the MVC pattern.


# Tech Stack
This project is built using the MERN stack and other modern web technologies.

-   **Backend**:
    -   [Node.js](https://nodejs.org/)
    -   [Express.js](https://expressjs.com/)
-   **Database**:
    -   [MongoDB](https://www.mongodb.com/)
    -   [Mongoose](https://mongoosejs.com/) (for object data modeling)
-   **Utilities**:
    -   [Nano ID](https://github.com/ai/nanoid) (for generating unique short IDs)
    

## Utilities:
Nodemon (for automatic server restarts during development)
Nano ID / ShortID (for generating unique short IDs)


# Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites
You must have the following installed on your machine:
- Node.js (which includes npm)
- MongoDB (Make sure the MongoDB server is running)

## Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/kirtishrestha/URL-SHORTNER.git
    ```

2.  **Navigate to the project directory:**
    ```bash
    cd URL-SHORTNER
    ```

3.  **Install dependencies:**
    ```bash
    npm install
    ```

4.  **Start the server:**
    ```bash
    npm start
    ```
    The API server will now be running on `http://localhost:8001`.


# API Endpoints
### 1. Generate a Short URL

-   **Endpoint**: `POST /url`
-   **Description**: Creates a new short URL.
-   **Request Body**:
    ```json
    {
      "url": "https://www.google.com"
    }
    ```
-   **Successful Response** (`200 OK`):
    ```json
    {
      "id": "A1b2C3d4"
    }
    ```

### 2. Redirect to Original URL

-   **Endpoint**: `GET /:shortId`
-   **Description**: Redirects to the original URL associated with the `shortId`.
-   **Example**: `http://localhost:8001/A1b2C3d4`
-   **Successful Response**: A `302 Found` redirect to the original URL.


# License
This project is licensed under the MIT License. See the LICENSE file for details.
