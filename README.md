# Book Store Management System

A full-stack book store application built with the MERN stack (MongoDB, Express.js, React, Node.js). This system helps you manage book inventory with a clean interface and solid backend architecture.

## Features

- Complete book CRUD operations - add, view, update, and delete books from your catalog
- RESTful API built with Express.js for clean data handling
- Responsive React frontend styled with Tailwind CSS
- MongoDB database with Mongoose for efficient data management
- Real-time updates for instant catalog changes
- CORS enabled for secure API access
- Vite for fast development and hot module replacement

## Tech Stack

### Frontend

- React 19 - Modern UI library
- React Router - Navigation and routing
- Axios - HTTP client for API calls
- Tailwind CSS - Utility-first styling
- Vite - Fast build tool and dev server
- React Icons - Icon library

### Backend

- Node.js - JavaScript runtime
- Express.js - Web application framework
- MongoDB - NoSQL database
- Mongoose - MongoDB object modeling
- CORS - Cross-origin resource sharing

## Prerequisites

Before running this project, make sure you have:

- Node.js (v18 or higher)
- MongoDB (v6 or higher)
- npm or yarn package manager

## Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd <project-directory>
```

### 2. Backend Setup

```bash
cd backend
npm install
```

Configure your MongoDB connection in `backend/config.js`:

```javascript
export const PORT = 5555;
export const mongoDBURL = "mongodb://127.0.0.1:27017/book_store";
```

### 3. Frontend Setup

```bash
cd frontend
npm install
```

## Running the Application

### Start MongoDB

Make sure MongoDB is running on your system:

```bash
mongod
```

### Start Backend Server

```bash
cd backend
npm run dev
```

The backend will run on `http://localhost:5555`

### Start Frontend Development Server

```bash
cd frontend
npm run dev
```

The frontend will run on `http://localhost:5173`

## Project Structure

```
.
├── backend/
│   ├── config.js           # Configuration settings
│   ├── index.js            # Express server entry point
│   ├── models/             # Mongoose data models
│   │   └── bookModel.js
│   ├── routes/             # API route handlers
│   │   └── booksRoute.js
│   └── package.json
│
├── frontend/
│   ├── src/                # React source files
│   ├── public/             # Static assets
│   ├── index.html          # HTML entry point
│   ├── vite.config.js      # Vite configuration
│   └── package.json
│
└── README.md
```

## API Endpoints

### Books

- `GET /books` - Retrieve all books
- `GET /books/:id` - Get a specific book
- `POST /books` - Add a new book
- `PUT /books/:id` - Update a book
- `DELETE /books/:id` - Delete a book

## Future Enhancements

We're planning to transform this into a multi-city digital library management system across India. The vision is to connect libraries in different cities so people can access books from anywhere, making public library resources more accessible and easier to manage.

Here's what we're working towards:

- Multi-city library network where users can browse and borrow books from any participating library
- Simple, intuitive interface for the public to search, reserve, and manage their borrowed books
- Inter-library book transfers to share resources efficiently between cities
- User accounts with reading history and personalized recommendations
- Administrative tools for librarians including inventory tracking, member management, and analytics
- Modern features like mobile apps, QR code checkout, and automated notifications

The idea is to make library resources available to more people across India while making day-to-day management smoother for library staff.

## Contributing

Contributions are welcome! If you'd like to help improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## Development Roadmap

- [x] Phase 1: Core book management (Current)
- [ ] Phase 2: User authentication and member profiles
- [ ] Phase 3: Multi-library and multi-city support
- [ ] Phase 4: Public reservation and borrowing system
- [ ] Phase 5: Administrative dashboard and analytics
- [ ] Phase 6: Mobile application and advanced features

## License

ISC

## Support

If you run into any issues or have questions, feel free to open an issue in the repository.

---

**Note**: This project is under active development. The multi-city features are being implemented in phases to ensure robust, scalable, and user-friendly operation across India's diverse library network.
