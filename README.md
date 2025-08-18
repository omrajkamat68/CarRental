# 🚗 CarRentX – Car Rental Marketplace (MERN + Vite + Tailwind)

**CarRentX** is a feature-rich **MERN stack** application that offers a seamless car rental experience. Users can sign up, explore cars, book them by location and dates, and manage their bookings. Owners get a powerful dashboard to list cars, manage availability, bookings, and view revenue insights.

---

## 🚀 **Live Demo**

🌐 Click here to explore the deployed app:
🔗 **[https://car-rental-client-pi.vercel.app/](https://car-rental-client-pi.vercel.app/)**

---

## 🚀 Key Features

### 👤 User Experience

* 🔐 **Secure Authentication**

  * Sign up / login using JWT
  * Protected routes with persistent sessions

* 🚘 **Car Discovery & Booking**

  * Browse cars with images, features, location, and price/day
  * Filter cars by **model, location, or features**
  * Enter **pickup & return date** to book instantly

* 📒 **My Bookings**

  * View all bookings with status: Pending, Confirmed, Cancelled
  * Access complete booking history

---

### 🧑‍💼 Owner Dashboard

* 📊 **Dashboard Overview**

  * Total Cars
  * Total Bookings
  * Pending vs Confirmed
  * Recent Bookings
  * Monthly Revenue

* ➕ **Add Car**

  * Create listings with brand, model, features, price/day, images, and location

* 🛠️ **Manage Cars**

  * Toggle availability on/off
  * Delete cars when needed

* 📑 **Manage Bookings**

  * Confirm or cancel customer bookings

* 🧑‍🎨 **Profile Management**

  * Upload/change profile picture using ImageKit

---

## 🧪 Tech Stack

| 🧰 Technology   | 📝 Description                         |
| --------------- | -------------------------------------- |
| 🟢 MongoDB      | Database (NoSQL)                       |
| ⚙️ Express.js   | Backend Framework                      |
| ⚛️ React + Vite | Frontend Framework (SPA)               |
| 🟣 Node.js      | JavaScript Runtime                     |
| 🎨 Tailwind CSS | Utility-first CSS Framework            |
| 🔐 JWT          | Authentication & Authorization         |
| 🖼️ ImageKit    | Image Upload & Optimization            |
| ☁️ Vercel       | Client Deployment                      |

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
git clone <your-repo-url> car-rental
cd car-rental
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
npm run dev
```

🚀 **Start Frontend:**

```bash
cd client
npm run dev
```

Open frontend at: **[http://localhost:5173](http://localhost:5173)**

---

## 🧯 Troubleshooting

* **CORS blocked?**
  Ensure server CORS allows your client origin:

  ```
  Access-Control-Allow-Origin: http://localhost:5173
  ```

* **Unauthorized / 401?**

  * Missing/invalid **Bearer token**
  * **JWT\_SECRET** mismatch

* **Images not showing?**

  * Verify ImageKit keys and endpoint

* **Bookings overlap incorrectly?**
  Ensure condition:

  ```
  newPickup <= existingReturn AND newReturn >= existingPickup
  ```

* **Search returns nothing?**

  * Check DB indexes (model, location, features)
  * Inspect query params in client & API

---

## 🚀 Deployment

### Client (Vercel)

* Import repo → add **client .env vars**
* `npm run build` → Vercel auto-detects Vite
* Ensure `VITE_BASE_URL` points to live server

### Server (Render/Railway/Fly/Heroku)

* Add env vars from `server/.env`
* Expose port `3000`
* Enable **CORS** for client origin

### MongoDB Atlas

* Create DB & user with least privileges
* Add server IP → avoid `0.0.0.0/0` in production

### ImageKit

* Setup project, URL endpoint, keys
* Use SDK for uploads or signed client uploads

---

## 🧭 UX Highlights

* Responsive **Tailwind UI**
* Debounced search & filters
* Informative **empty states** & toasts
* Accessible forms with validation
* Clean car & booking cards

---

## 🗺️ Roadmap

* 💳 Payment Integration (Stripe/Razorpay)
* ⭐ Reviews & Ratings
* 🧾 Invoices & Owner Payouts
* 🌍 Multi-currency & i18n
* 🛰️ Real-time availability (WebSockets)
* 🧠 Advanced pricing (weekend/seasonal)

---

## 📸 Screenshots (Optional)

*Add screenshots/GIFs here:*

* Home / Search
* Cars Catalog
* Car Details + Booking
* My Bookings
* Owner Dashboard
* Manage Cars / Bookings

---

## 🙌 Acknowledgements

* **MongoDB Atlas** — Managed Database
* **ImageKit** — Media storage & CDN
* **React + Vite** — Fast SPA Framework
* **Tailwind CSS** — Utility-first styling

---

## 📜 License

MIT — free to use, fork, and expand.

---

## 👤 Author

**Omraj Kamat**
🌐 Live App: **[https://car-rental-client-pi.vercel.app/](https://car-rental-client-pi.vercel.app/)**

*For feedback or collaboration, please open an issue or reach out via your preferred channel.*
