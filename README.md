# MERN Course Project

This project is a full-stack application built using the MERN stack (MongoDB, Express, React, Node.js). It includes a backend server and a frontend client, providing a complete web application experience.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [Contributing](#contributing)
- [License](#license)

## Installation

### Prerequisites

- Node.js (version 16.x recommended)
- npm or yarn
- MongoDB

### Backend Setup

1. Navigate to the backend directory:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables by creating a `.env` file in the `backend` directory. Use the following template:

   ```env
   MONGO_CONNECTION_STRING=your_mongo_connection_string
   SESSION_SECRET=your_session_secret
   PORT=5000
   ```

4. Start the backend server:

   ```bash
   npm start
   ```

### Frontend Setup

1. Navigate to the frontend directory:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the frontend development server:

   ```bash
   npm start
   ```

## Usage

- Access the application by navigating to `http://localhost:3000` in your web browser.
- The backend server runs on `http://localhost:5000`.

## Features

- **User Authentication**: Sign up, log in, and log out functionality.
- **Note Management**: Create, edit, and delete notes.
- **Responsive Design**: Built with React Bootstrap for a responsive user interface.
- **Error Handling**: Custom error pages for not found and privacy policy.
- **Session Management**: Secure session handling with express-session and MongoDB.

## Project Structure

### Backend

- `src/app.ts`: Express application setup and middleware configuration.
- `src/server.ts`: Server entry point, connects to MongoDB and starts the server.
- `src/routes`: API routes for users and notes.
- `src/controllers`: Request handlers for business logic.
- `src/models`: Mongoose models for database schemas.
- `src/middleware`: Custom middleware for authentication and error handling.

### Frontend

- `src/App.tsx`: Main application component, sets up routing and context providers.
- `src/components`: Reusable React components.
  - `NavBarLoggedOutView.tsx`: Navigation bar for logged-out users.
  - `NotesPageLoggedOutView.tsx`: View for notes page when user is not logged in.
  - `NotesPageLoggedInView.tsx`: View for notes page when user is logged in.
  - `Note.tsx`: Component to display individual notes.
  - `AddEditNoteDialog.tsx`: Dialog for adding or editing notes.
  - `SignUpModal.tsx`: Modal for user sign-up.
- `src/pages`: Page components for different routes.
  - `PrivacyPage.tsx`: Privacy policy page.
  - `NotFoundPage.tsx`: 404 error page.

## Environment Variables

The project requires the following environment variables:

- `MONGO_CONNECTION_STRING`: MongoDB connection string
- `SESSION_SECRET`: Secret key for session management
- `PORT`: Port number for the backend server

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
