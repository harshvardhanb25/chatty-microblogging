# Chatty — Microblogging Platform

A simple microblogging web application built with **Node.js**, **Express**, and **MongoDB**. Originally developed as a final project for **CSC-337 at the University of Arizona**.

---

## Features

- User registration and session-based authentication
- Create, view, and delete posts (microblogs)
- Input validation and sanitization (via `express-validator` and `mongo-sanitize`)
- File upload support with `formidable`
- Persistent sessions stored in MongoDB via `connect-mongo`

---

## Tech Stack

| Layer      | Technology                        |
|------------|-----------------------------------|
| Runtime    | Node.js                           |
| Framework  | Express.js                        |
| Database   | MongoDB + Mongoose                |
| Sessions   | express-session + connect-mongo   |
| Testing    | Mocha + Chai                      |
| Dev Tools  | nodemon, dotenv                   |

---

## Getting Started

### Prerequisites

- Node.js (v16+)
- MongoDB instance (local or Atlas)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/harshvardhanb25/chatty-microblogging.git
   cd chatty-microblogging
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment variables**

   Copy the template and fill in your values:
   ```bash
   cp .env.template .env
   ```

4. **Start the server**
   ```bash
   npm start
   ```

   The app will be available at `http://localhost:3000` by default.

---

## Running Tests

```bash
npm test
```

Tests are written using **Mocha** and **Chai** and located in the `tests/` directory.

---

## Project Structure

```
chatty-microblogging/
├── middleware/        # Custom Express middleware
├── models/            # Mongoose schemas/models
├── public_html/       # Static frontend assets
├── tests/             # Mocha/Chai test files
├── server.js          # App entry point
├── config.js          # Configuration helpers
├── .env.template      # Environment variable template
└── package.json
```

---

## License

This project is unlicensed and was created for educational purposes.
