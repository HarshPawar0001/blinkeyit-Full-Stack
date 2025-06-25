
````markdown
# Blinkeyit – Blinkit-like E-commerce Platform

![Project Preview](Thumnails.png?raw=true "Project Preview")

## About

Blinkeyit is a modern, full-stack e-commerce platform built using the MERN stack  
(MongoDB, Express.js, React, Node.js) that emulates the core features and user  
experience of popular online grocery delivery services like Blinkit.

It offers secure user authentication with OTP verification, Stripe-based payment  
integration, an intuitive shopping experience, and a powerful admin dashboard  
for managing products, categories, orders, and users.

The project emphasizes clean architecture, scalable backend APIs, and a mobile-first,  
responsive frontend — making it an ideal portfolio-grade application for showcasing  
real-world full-stack development skills.

---

## Table of Contents

- Features  
- Tech Stack  
- Getting Started  
- Installation  
- Running the App  
- Usage Guide  
- Directory Structure  
- Security  
- Payments  
- Admin Panel  
- Contributing  
- License  
- Contact  

---

## Features

**User Authentication**  
- JWT-based Access & Refresh Tokens  
- OTP Email Verification  
- Password Recovery  

**Product & Category Management**  
- Admin CRUD for Products  
- Cloudinary Image Storage  
- Categorized & Subcategorized Listings  

**Shopping Cart & Orders**  
- Persistent Cart  
- Order Placement & History  

**Admin Dashboard**  
- Product, Category, User & Order Management  

**Stripe Integration**  
- Secure Online Payments  

**Responsive UI**  
- Tailwind CSS & SweetAlert2  

**Transactional Emails**  
- OTP & Recovery via Resend  

**API Testing**  
- Postman-ready APIs  

---

## Tech Stack

### Frontend
- React.js with Vite  
- Redux Toolkit  
- React Router  
- Axios  
- Tailwind CSS  
- SweetAlert2  

### Backend
- Node.js with Express.js  
- MongoDB + Mongoose  
- JWT (Access + Refresh Tokens)  
- Cloudinary  
- Stripe  
- Resend  
- Dotenv  

---

## Getting Started

### Prerequisites

- Node.js (LTS version recommended)  
- npm or Yarn  
- MongoDB (local or Atlas)  
- Cloudinary Account  
- Stripe Account  
- Resend Account  

---

## Installation

```bash
# Clone the repository
git clone https://github.com/HarshPawar0001/blinkeyit-Full-Stack.git
cd blinkeyit-Full-Stack
````

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the `backend/` directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
JWT_ACCESS_TOKEN_SECRET=your_access_token_secret
JWT_REFRESH_TOKEN_SECRET=your_refresh_token_secret
JWT_ACCESS_TOKEN_EXPIRATION=1h
JWT_REFRESH_TOKEN_EXPIRATION=7d
CLOUD_NAME=your_cloudinary_cloud_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=no-reply@yourdomain.com
```

---

### Frontend Setup

```bash
cd ../frontend
npm install
```

Create a `.env` file in the `frontend/` directory:

```env
VITE_API_URL=http://localhost:5000/api/v1
```

---

## Running the App

### In two terminals:

```bash
# Terminal 1 - Backend
cd backend
npm start
```

```bash
# Terminal 2 - Frontend
cd frontend
npm run dev
```

* Backend URL: [http://localhost:5000](http://localhost:5000)
* Frontend URL: [http://localhost:5173](http://localhost:5173)

---

## Usage Guide

* Register a new user (OTP email verification)
* Log in to access user dashboard
* Browse products by category/subcategory
* Add to cart and proceed to checkout (Stripe)
* Admins can manage products, users, orders, and categories

---

## Directory Structure

```plaintext
blinkeyit-Full-Stack/
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   └── server.js
└── frontend/
    ├── public/
    ├── src/
    │   ├── assets/
    │   ├── components/
    │   ├── pages/
    │   ├── redux/
    │   ├── services/
    │   ├── hooks/
    │   ├── App.jsx
    │   └── main.jsx
    └── tailwind.config.js
```

---

## Security

* Access Tokens: Short-lived, memory-stored
* Refresh Tokens: Long-lived, HttpOnly cookies
* OTP Verification: Prevents fake sign-ups

---

## Payments

* Integrated with Stripe
* Secure card handling and payment confirmation

---

## Admin Panel

* Product Management (CRUD)
* Category/Subcategory Management
* User View/Block
* Order Fulfillment and Tracking

---

## Contributing

```bash
# Fork the repository
# Create your feature branch
git checkout -b feature/YourFeature

# Commit your changes
git commit -m "Add YourFeature"

# Push to GitHub
git push origin feature/YourFeature

# Open a Pull Request
```

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

* GitHub: [HarshPawar0001](https://github.com/HarshPawar0001)
* Email: [harsh.pawar.ug23@nsut.ac.in](mailto:harsh.pawar.ug23@nsut.ac.in)

```

