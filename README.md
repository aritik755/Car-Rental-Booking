# 🚗 Car Rental Booking Website

🔗 **Live Demo:** (https://car-rental-lac-nu.vercel.app/)

A full-stack car rental booking platform built using the **MERN stack** that allows users to browse available cars, book vehicles, manage reservations, and manage car listings through an owner dashboard.

## ✨ Features

### 👤 User Features

- Browse available cars and view car details.
- Search cars by location and booking dates.
- Book cars for selected dates.
- View and manage personal bookings.
- Manage user profile and profile image.

### 🛠️ Owner Features

- Switch to owner mode.
- Add and manage car listings.
- Upload car images.
- Toggle car availability.
- View customer bookings.
- Update booking status through the dashboard.

### 🔐 Security & Authentication

- User authentication using JWT.
- Password hashing using bcrypt.
- Protected API routes.
- Role-based access for car owners.
- Environment variables for sensitive configuration.

## 🧰 Tech Stack

**Frontend**

- React.js
- Vite
- React Router
- Axios
- Tailwind CSS
- Motion (Animations & Transitions)

**Backend**

- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- bcrypt
- Multer

**Image Management**

- ImageKit

## 📁 Project Structure

```text
Car Rental Booking Website/
├── client/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── .env
├── server/
│   ├── configs/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── package.json
│   └── .env
├── .gitignore
└── README.md
```

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd "Car Rental Booking Website"
```

### 2. Set Up the Backend

```bash
cd server
npm install
```

Create a `.env` file inside the `server` directory and configure:

```env
PORT=3000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
```

Use the port and variable names expected by your actual server configuration.

Start the backend:

```bash
npm run server
```

If your project uses a different script, check `server/package.json`.

### 3. Set Up the Frontend

Open another terminal:

```bash
cd client
npm install
```

Create a `.env` file inside the `client` directory:

```env
VITE_BASE_URL=http://localhost:3000
VITE_CURRENCY=₹
```

Ensure `VITE_BASE_URL` matches the port and URL of your backend.

Start the frontend:

```bash
npm run dev
```

Open the local URL displayed by Vite in your terminal.

## 🔌 API Overview

| Endpoint        | Description                       |
| --------------- | --------------------------------- |
| `/api/user`     | User authentication and profile   |
| `/api/owner`    | Car listings and owner operations |
| `/api/bookings` | Booking operations                |
| `/api/food`     | Not used in this project          |

> The API routes above represent the main route groups. Individual endpoints depend on your implementation.

## 🔑 Environment Variables

Keep all API keys, database credentials, and JWT secrets in environment files. Never commit real `.env` files to GitHub.

## 🚀 Future Improvements

- Online payment integration.
- Email booking confirmations.
- Advanced filtering and sorting.
- Booking history and cancellation.
- Responsive UI improvements.
- Deployment with a live database.

## 👨‍💻 Author

**Ritik Agarwal**

B.Tech – Information Technology

GitHub: (https://github.com/aritik755)

---

⭐ If you find this project useful, consider giving the repository a star!
