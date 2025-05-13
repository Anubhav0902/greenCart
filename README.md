# 🌿 GreenCart – Your Online Grocery Store

GreenCart is a full-stack e-commerce application built with the **MERN stack** (MongoDB, Express, React, Node.js) featuring:

- 🛒 Product Listings & Cart  
- 🔐 JWT-based Auth for Users & Sellers  
- 💳 Stripe Payment Integration  
- ☁️ Cloudinary Image Upload  
- 🌐 Deployed on Vercel (Frontend) and Backend (e.g. Railway/Render)

---

## 📸 Demo

👉 [Live App](https://greencart-rose.vercel.app)  
Try logging in or registering to experience full features.

---

## ⚙️ Tech Stack

| Technology     | Used For               |
|----------------|------------------------|
| MongoDB        | Database               |
| Express.js     | Backend API            |
| React.js       | Frontend UI            |
| Node.js        | Server-side JS         |
| Cloudinary     | Image Uploads          |
| Stripe         | Payment Gateway        |
| Vercel         | Frontend Deployment    |
| GitHub         | Version Control        |
| JWT & Cookies  | Auth & Sessions        |

---

## 🧩 Features

### 👤 Authentication
- Register/Login for users
- JWT + HttpOnly Cookies
- Separate login for sellers

### 🛍️ E-Commerce
- Product upload (by sellers)
- Product listing with images
- Add to cart, checkout

### 💳 Payments
- Stripe checkout session
- Handles success/cancel redirects

### 📦 Orders
- Place orders
- Track order history

### 📤 Cloudinary
- Upload product images
- Store secure image URLs

---

## 🚀 Setup Instructions

### 📁 Clone the repo

```bash
git clone https://github.com/your-username/greenCart.git
cd greenCart
```

### ⚙️ Backend Setup
```
cd server
npm install
```

### Create .env file
```
PORT=4000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret
NODE_ENV=development
```

```
npm run start
```

### 💻 Frontend Setup
```
cd frontend
npm install
npm run dev
```

### Make sure Axios is configured with:
```
withCredentials: true
```

--- 

### 🔐 Auth Flow
- User registers or logs in
- Server sets JWT in an HttpOnly Cookie
- On page refresh, /api/user/is-auth checks cookie for login state

---

### 🧪 Testing Stripe Payments
- You must use a Stripe Business Account (India) and configure your keys properly.
- Use Stripe test card: 4242 4242 4242 4242 – Any future expiry date, any CVC.

---

### 🧠 Folder Structure
```
greenCart/
│
├── backend/
│   ├── configs/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   └── server.js
│
├── frontend/
│   ├── components/
│   ├── context/
│   ├── pages/
│   └── App.jsx
│
└── README.md
```

---

### 🔒 Security Notes
- .env is added to .gitignore
- Make sure not to upload secrets to GitHub
- Use secure cookies in production:

```
secure: true
sameSite: "none"
```

--- 


### 📦 Deployment
- Frontend: Vercel
- Backend: Vercel or Any Node.js-supported platform (e.g. Render, Railway)

---

### 🤝 Contributing
Feel free to fork the project and submit PRs. Contributions are welcome!

---

### 📧 Contact
Made with ❤️ by Anubhav
