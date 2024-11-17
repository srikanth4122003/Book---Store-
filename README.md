
# 📚 MERN Stack Book Store Application

This is a full-stack web application built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. The application provides an online platform where users can browse, buy, and manage books while sellers can list books for sale.

## 🌟 Features

### User Features
- 📖 Browse books by category, author, or genre.
- 🛒 Add books to a shopping cart and proceed to purchase.
- ❤️ Add books to a wishlist for future reference.
- 📦 View and manage past orders.

### Seller Features
- 📝 Create an account and log in as a seller.
- 📚 List books for sale with details like title, author, genre, description, and price.
- ✏️ Manage listed books (update/delete listings).
- 📦 View orders placed by users for their books.

### Admin Features
- 🔑 Secure login for admin users.
- 🧑‍💻 Manage users, sellers, and their activities.
- 🗑️ Delete inappropriate books or user accounts.

---

## 🛠️ Technologies Used

### Frontend
- **React.js**: User interface with dynamic rendering.
- **Axios**: For making HTTP requests to the backend.
- **Bootstrap**: Styling for responsive UI.

### Backend
- **Node.js**: Server-side runtime environment.
- **Express.js**: Framework for building RESTful APIs.
- **Multer**: File upload handling for images (e.g., book covers).

### Database
- **MongoDB**: NoSQL database for storing users, books, orders, and wishlist data.
- **Mongoose**: Object Data Modeling (ODM) for MongoDB and Node.js.

---

## 🚀 Installation and Setup

### Prerequisites
- Node.js and npm installed
- MongoDB running locally or MongoDB Atlas account
- Git for version control

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/srikanth4122003/Book---Store-.git
   cd Book---Store
   ```

2. **Install Backend Dependencies**
   ```bash
   cd backend
   npm install
   ```

3. **Set Up Environment Variables**
   Create a `.env` file in the backend folder with the following details:
   ```makefile
   PORT=4000
   MONGO_URI=mongodb://localhost:27017/bookstore
   JWT_SECRET=your_secret_key
   ```

4. **Run the Backend Server**
   ```bash
   npm start
   ```
   The backend server will run on `http://localhost:4000`.

5. **Install Frontend Dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

6. **Start the Frontend Server**
   ```bash
   npm start
   ```
   The frontend server will run on `http://localhost:5173` (or a different port based on your setup).

---

## 📂 Project Structure

### Backend (`/backend`)
- `/db`: Database connection and schemas.
- `/routes`: API routes for users, sellers, admin, books, etc.
- `/uploads`: Folder for storing book images.
- `server.js`: Main entry point for the backend server.

### Frontend (`/frontend`)
- `/src`: React components, pages, and styles.
- `/public`: Static files like images and favicon.

---

## 📋 API Endpoints

### User Routes
- `POST /signup`: Register a new user.
- `POST /login`: Log in an existing user.
- `GET /item`: Fetch all books.
- `POST /wishlist/add`: Add a book to the wishlist.

### Seller Routes
- `POST /ssignup`: Register a new seller.
- `POST /slogin`: Log in an existing seller.
- `POST /items`: Add a new book.

### Admin Routes
- `POST /asignup`: Register a new admin.
- `POST /alogin`: Log in an admin.
- `GET /users`: Get a list of all users.

---

## 🤝 Contributions
Contributions are welcome! If you’d like to contribute, please fork the repository and submit a pull request.

---

## 🧑‍💻 Authors
- **A.Srikanth** - Project Lead

---

## 📄 License
This project is licensed under the MIT License.
