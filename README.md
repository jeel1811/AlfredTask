# Flashcard Learning App

## Description
This is a full-stack web application for managing flashcards using the Leitner System. It features a MongoDB backend with Express.js and a React frontend.

## Features
- **Leitner System Implementation**
  - Automatic review scheduling
  - Multiple review boxes with increasing intervals
- **User Authentication**
  - Registration
  - Login
  - Password reset
- **Flashcard Management**
  - Create
  - Read
  - Update
  - Delete
- **Responsive Design**
  - Mobile-friendly interface
  - Dark mode support
- **Statistics Tracking**
  - Box statistics
  - Review history

## Getting Started

### Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/jeel1811/AlfredTask.git
   ```
2. **Install dependencies**:
   ```bash
   cd flashcard-app
   npm install
   cd frontend
   npm install
   ```
3. **Set up environment variables**:
   - Create `.env` files in both backend and frontend directories
     
   **Backend (`.env`)**:
   ```env
   PORT=8000
   MONGODB_URI="MongoDB URI"
   JWT_SECRET=Your_tocken
   ```
   **Frontend (`.env`)**:
   ```env
   REACT_APP_API_URL=http://localhost:8000/api
   ```

4. **Start MongoDB**:
   ```bash
   sudo service mongod start
   ```

5. **Start the application**:
   - Backend:
     ```bash
     cd backend
     node server.js
     ```
   - Frontend (in another terminal):
     ```bash
     cd frontend
     npm start
     ```

### Usage
- Access the application at `http://localhost:3000`
- Register a new user
- Login to access flashcard management
- Add new flashcards through the interface
- Review flashcards according to the Leitner System schedule

## Project Structure
```plaintext
flashcard-app/
├── backend/
│   ├── package.json
│   ├── server.js
│   ├── models/
│   │   ├── Flashcard.js
│   │   └── User.js
│   ├── routes/
│   │   ├── flashcardRoutes.js
│   │   └── userRoutes.js
│   └── middleware/
│       └── auth.js
├── frontend/
│   ├── package.json
│   ├── public/
│   │   ├── index.html
│   │   └── manifest.json
│   ├── src/
│   │   ├── App.tsx
│   │   ├── components/
│   │   │   ├── FlashcardList.tsx
│   │   │   └── AddFlashcard.tsx
│   │   └── contexts/
│   │       └── ThemeContext.tsx
└── README.md
```

## Contributing
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Run tests
5. Submit a pull request

## Author
Jeel Hirani  
[GitHub](https://github.com/jeel1811/)
