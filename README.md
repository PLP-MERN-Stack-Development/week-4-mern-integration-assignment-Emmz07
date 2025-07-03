Collecting workspace information```md
# MERN Blog Application

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) blog application demonstrating seamless integration between front-end and back-end components, including database operations, API communication, authentication, and state management.

## 📦 Project Structure

```
mern-blog/
├── client/                 # React front-end (Vite)
│   ├── my-app/             # Main React app
│   │   ├── public/         # Static files
│   │   ├── src/            # React source code
│   │   │   ├── components/ # Reusable components (to be implemented)
│   │   │   ├── pages/      # Page components (to be implemented)
│   │   │   ├── services/   # API services
│   │   │   └── App.jsx     # Main application component
│   │   └── package.json    # Client dependencies
├── server/                 # Express.js back-end
│   ├── config/             # Configuration files
│   ├── controller/         # Route controllers
│   ├── models/             # Mongoose models
│   ├── routes/             # API routes
│   ├── middleware/         # Custom middleware (to be implemented)
│   ├── utils/              # Utility functions (to be implemented)
│   ├── server.js           # Main server file
│   └── package.json        # Server dependencies
├── .github/                # GitHub Classroom & CI config
├── README.md               # Project documentation
└── Week4-Assignment.md     # Assignment instructions
```

## 🚀 Features

- RESTful API for blog posts and categories
- User authentication (register, login)
- CRUD operations for posts and categories
- MongoDB database integration with Mongoose
- React front-end with React Router
- API service layer for client-server communication
- Environment variable configuration
- Error handling and validation (to be expanded)
- Ready for advanced features: image uploads, comments, pagination, etc.

## 🛠️ Setup Instructions

### Prerequisites

- Node.js (v18+)
- MongoDB (local or Atlas)
- npm

### 1. Clone the Repository

```sh
git clone <your-repo-url>
cd week-4-mern-integration-assignment-Emmz07
```

### 2. Set Up the Server

```sh
cd server
cp .env.example .env   # If .env.example exists, otherwise edit .env
npm install
npm run dev            # or: node server.js
```

- Edit `.env` with your MongoDB URI and JWT secret.

### 3. Set Up the Client

```sh
cd ../client/my-app
npm install
npm run dev
```

- The client will run on [http://localhost:5000](http://localhost:5000) by default.

## 🌐 API Documentation

### Authentication

- `POST /api/auth/register` — Register a new user
- `POST /api/auth/login` — Login and receive JWT

### Posts

- `GET /api/posts` — Get all posts
- `GET /api/posts/:id` — Get a single post by ID
- `POST /api/posts` — Create a new post
- `PUT /api/posts/:id` — Update a post
- `DELETE /api/posts/:id` — Delete a post

### Categories

- `GET /api/categories` — Get all categories
- `POST /api/categories` — Create a new category

## 📝 Environment Variables

Example `.env` for the server:

```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/mern_integration
JWT_SECRET=your_secret_key
```

## 📸 Screenshots

_Add screenshots of your application here after implementation._

## 📄 Assignment

See [Week4-Assignment.md](Week4-Assignment.md) for detailed requirements and submission instructions.

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

## 📚 Resources

- [MongoDB Docs](https://docs.mongodb.com/)
- [Express.js Docs](https://expressjs.com/)
- [React Docs](https://react.dev/)
- [Node.js Docs](https://nodejs.org/en/docs/)
- [Mongoose Docs](https://mongoosejs.com/docs/)

---

_This project is part of a MERN stack integration assignment._
```
