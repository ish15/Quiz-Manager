# Quiz-Application

## Overview

This project is a Quiz-Application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The application features two portals: one for administrators and one for users.

- **Admin Portal**: Allows admins to create, modify, and delete quizzes, add and modify questions and answers, and view reports on user performance.
- **User Portal**: Allows users to register, log in, take quizzes, view results, and see the correct answers after completing the quizzes.

## Features

### Admin Portal
- Create quizzes
- Add questions to quizzes
- Modify quizzes and questions
- Modify answers
- View reports of all users

### User Portal
- Register and log in
- Attempt quizzes
- View results
- View correct answers after quiz completion

## Prerequisites

Ensure you have the following installed on your machine:
- Node.js
- npm (Node Package Manager)
- MongoDB Atlas account (for cloud database)

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/quiz-application.git
cd quiz-application
```

### 2. Set Up MongoDB

- Sign up for a [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) account.
- Create a new cluster.
- Get your MongoDB connection string. It should look something like this:

  ```plaintext
  mongodb+srv://<Name>:<Password>@cluster0.mongodb.net/<YourDBName>?retryWrites=true&w=majority
  ```

- Create a `.env` file in the root directory and add your MongoDB connection string:

  ```plaintext
  MONGO_URI=mongodb+srv://<Name>:<Password>@cluster0.mongodb.net/<YourDBName>?retryWrites=true&w=majority
  ```

### 3. Install Server Dependencies

In the root directory, run:

```bash
npm install
```

### 4. Run the Server

```bash
npm start
```

The server will start running on `http://localhost:3000`.

### 5. Install Client Dependencies

Open another terminal, navigate to the client directory, and run:

```bash
cd client
npm install
```

### 6. Run the Client

```bash
npm start
```

The client will start running on `http://localhost:3001`.

## Usage

### Admin Portal

1. Open your browser and navigate to `http://localhost:3001/admin`.
2. Log in with your admin credentials.
3. Use the dashboard to create, modify, and manage quizzes and questions.
4. View user reports and performance.

### User Portal

1. Open your browser and navigate to `http://localhost:3001`.
2. Register a new account or log in with your existing credentials.
3. Select a quiz to attempt.
4. Answer the questions and submit the quiz.
5. View your results and see the correct answers after completing the quiz.

## Project Structure

```
quiz-application/
├── client/               # React frontend
│   ├── public/           # Public assets
│   ├── src/              # Source files
│   └── ...               # Other configuration files
├── server/               # Express backend
│   ├── config/           # Configuration files
│   ├── controllers/      # Route handlers
│   ├── models/           # Mongoose models
│   ├── routes/           # API routes
│   └── ...               # Other configuration files
├── .env                  # Environment variables
├── package.json          # npm package configuration
└── ...                   # Other configuration files
```

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.
