# 🚗 Car Rental Website (MERN + Vite + Tailwind)

**CarRental** is a modern **MERN stack** application that delivers a seamless car rental experience. Customers can explore cars, book them by location and dates, and manage bookings, while owners can list cars, manage availability, handle bookings, and view revenue insights through a powerful dashboard.

---

## 🚀 **Live Demo**

✨ **Click here to explore the deployed app:**
👉 🔗 (https://car-rental-client-pi.vercel.app/) 👈

---

## 🚀 Key Features

### 👤 User Experience

* 🔐 **Secure Authentication**

  * Sign up / login with JWT
  * Protected routes with persistent sessions

* 🚘 **Car Discovery & Booking**

  * Browse cars with photos, features, location, and daily pricing
  * Search & filter by **model, location, or features**
  * Book instantly by selecting **pickup & return dates**

* 📒 **My Bookings**

  * View booking history with statuses: **Pending, Confirmed, Cancelled**
  * Track all upcoming and past bookings

---

### 🧑‍💼 Owner Dashboard

* 📊 **Dashboard Overview**

  * Total Cars
  * Total Bookings
  * Pending vs Confirmed
  * Recent Bookings
  * Monthly Revenue

* ➕ **Add Car**

  * Add cars with brand, model, features, daily price, location, and images

* 🛠️ **Manage Cars**

  * Toggle availability status
  * Delete cars when required

* 📑 **Manage Bookings**

  * Approve/Confirm or Cancel bookings

* 🧑‍🎨 **Profile Management**

  * Upload/change profile image using **ImageKit**

---

## 🧪 Tech Stack

| 🧰 Technology   | 📝 Description                 |
| --------------- | ------------------------------ |
| 🟢 MongoDB      | Database (NoSQL)               |
| ⚙️ Express.js   | Backend Framework              |
| ⚛️ React + Vite | Frontend Framework (SPA)       |
| 🟣 Node.js      | JavaScript Runtime             |
| 🎨 Tailwind CSS | Utility-first CSS Framework    |
| 🔐 JWT          | Authentication & Authorization |
| 🖼️ ImageKit    | Image Upload & Optimization    |
| ☁️ Vercel       | Client & Server Deployment              |

---

## 🔐 Environment Variables

### 🌐 Server-Side (`server/.env`)

```
MONGODB_URI=
JWT_SECRET=

IMAGEKIT_PUBLIC_KEY=
IMAGEKIT_PRIVATE_KEY=
IMAGEKIT_URL_ENDPOINT=
```

### 💻 Client-Side (`client/.env`)

```
VITE_CURRENCY=$
VITE_BASE_URL=http://localhost:3000
```

---

## 🧾 Local Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/omrajkamat68/CarRental.git
cd CarRental
```

### 2️⃣ Install Dependencies

📦 **Backend:**

```bash
cd server
npm install
```

📦 **Frontend:**

```bash
cd ../client
npm install
```

### 3️⃣ Run the Application

🚀 **Start Backend:**

```bash
cd server
npm run server
```

🚀 **Start Frontend:**

```bash
cd client
npm run dev
```
---

## 🧠 Core Logic Highlights

* ⏱️ **Booking Conflict Prevention:** Prevents overlapping reservations
* 📊 **Revenue Insights:** Monthly revenue calculated with MongoDB aggregation
* 🚦 **Availability Toggle:** Owners can switch car availability anytime

---

## 🌟 Future Enhancements

* 💳 Payment Integration (Stripe/Razorpay)
* ⭐ Ratings & Reviews
* 🧾 Invoices & Owner Payouts
* 🌍 Multi-currency & Multi-language support
* 🛰️ Real-time Availability (WebSockets)
* 🧠 Advanced Pricing Models (Weekend/Seasonal)

---

## 🙌 Acknowledgements

* **MongoDB Atlas** — Managed Database
* **ImageKit** — Media Storage & CDN
* **React + Vite** — Fast Frontend Framework
* **Tailwind CSS** — Utility-first Styling

---
