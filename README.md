# MERN Notes Application

A full-stack notes application built with the MERN stack (MongoDB, Express.js, React, Node.js) featuring a modern UI with dark mode support.

## 🚀 Features

- **CRUD Operations**: Create, Read, Update, and Delete notes
- **Modern UI**: Clean, responsive design with dark mode
- **Real-time Updates**: Instant note updates without page refresh
- **Rate Limiting**: Protected API endpoints with rate limiting
- **Responsive Design**: Works on desktop and mobile devices
- **Toast Notifications**: User feedback for actions

## 🛠️ Tech Stack

### Frontend
- **React** - Frontend library
- **React Router** - Client-side routing
- **Tailwind CSS** - Styling with utility-first CSS
- **DaisyUI** - Component library for Tailwind CSS
- **Lucide Icons** - Beautiful & consistent icon toolkit
- **React Hot Toast** - Toast notifications
- **Axios** - HTTP client

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variables
- **Upstash Rate Limiting** - API rate limiting

## 📦 Prerequisites

- Node.js (v14+)
- npm or yarn
- MongoDB Atlas account or local MongoDB instance

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd MERN-Project
```

### 2. Set up the Backend

```bash
cd backend
npm install
```

Create a [.env](cci:7://file:///Users/shubham/MyTechData/MERN%20Project/backend/.env:0:0-0:0) file in the backend directory with the following variables:

```env
PORT=5001
MONGO_URI=your_mongodb_connection_string
UPSTASH_REDIS_REST_URL=your_upstash_redis_rest_url
UPSTASH_REDIS_REST_TOKEN=your_upstash_redis_rest_token
```

### 3. Set up the Frontend

```bash
cd ../frontend
npm install
```

### 4. Run the Application

#### Development Mode

In separate terminal windows:

```bash
# Start backend
cd backend
npm run dev

# Start frontend
cd ../frontend
npm run dev
```

The application will be available at `http://localhost:5173`

#### Production Mode

```bash
# Build the frontend
cd frontend
npm run build

# Start the production server
cd ../backend
npm start
```

## 🌐 API Endpoints

- `GET /api/notes` - Get all notes
- `GET /api/notes/:id` - Get a single note
- `POST /api/notes` - Create a new note
- `PUT /api/notes/:id` - Update a note
- `DELETE /api/notes/:id` - Delete a note

## 📂 Project Structure

```text
MERN-Project/
├── backend/
│   ├── src/
│   │   ├── config/
│   │   │   └── db.js          # Database connection
│   │   ├── controllers/       # Route controllers
│   │   ├── middleware/        # Custom middleware
│   │   ├── models/            # Mongoose models
│   │   ├── routes/            # API routes
│   │   └── server.js          # Express server setup
│   └── .env                   # Environment variables
│
├── frontend/
│   ├── public/                # Static files
│   └── src/
│       ├── components/        # Reusable UI components
│       ├── lib/               # Utility functions
│       ├── pages/             # Page components
│       ├── App.jsx            # Main App component
│       └── main.jsx           # Entry point
│
├── .gitignore
└── package.json
```

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Vite](https://vitejs.dev/) - Next Generation Frontend Tooling
- [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework
- [DaisyUI](https://daisyui.com/) - Component library for Tailwind CSS
- [Lucide Icons](https://lucide.dev/) - Beautiful & consistent icon toolkit
```
