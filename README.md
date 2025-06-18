# 🎥 BookFlix

**BookFlix** is a full-stack movie ticket booking application built with the **MERN stack**, providing an intuitive platform for users to browse movies, check seat availability, book tickets, and enjoy a seamless booking experience. It integrates **Clerk** for authentication, **Stripe** for secure payments, and uses **Ingest** and **Brevo** for transactional and promotional email notifications.

---

## 📌 Project Overview

- **Users** can browse movies, watch trailers, check real-time seat availability, book tickets, make payments via Stripe, and manage their bookings.
- **Admins** can manage shows, track total bookings, view revenue statistics, monitor seat availability per show, and send promotional announcements.

---

## ✨ Features

### 🏠 Public Homepage Features

- **Movie Listing with Trailers**
  - Browse available movies with posters, showtimes, and trailers.

- **Seat Availability Preview**
  - View real-time seat availability for each show before booking.

- **Secure Booking and Payments**
  - Book tickets and make payments via integrated **Stripe Payment Gateway**.

- **Favourites System**
  - Add movies to a favourites list for easy access.

---

### 🎟️ User Features

After securely logging in via **Clerk**, users can:

- **Browse and Explore Movies**
  - Access detailed information including trailers and show schedules.

- **Book Movie Tickets**
  - Check available seats for a show in real-time.
  - Select seats and complete booking using **Stripe**.

- **Booking Management**
  - View booking history with details like seat numbers, show time, and status.

- **Receive Email Notifications**
  - Booking confirmations
  - New show announcements
  - Show reminders

- **Favourites Management**
  - Add and manage favourite movies for easy future bookings.

---

### 🛠️ Admin Features

Admins accessing the admin portal can:

- **Add New Shows**
  - Add movies with show details, timing, available seats, and ticket pricing.

- **Manage Seat Availability**
  - Track and update available seats in real-time to prevent overbooking.

- **View Booking Details**
  - Access a comprehensive list of bookings for each show.

- **Revenue and Stats Dashboard**
  - Monitor total revenue, active shows, and total registered users.

- **Send Promotional Emails**
  - Announce new shows or offers via integrated email services.

---

## 📊 Email Notifications

**BookFlix** uses **Ingest** for transactional emails (e.g., booking confirmations, show reminders) and **Brevo (Sendinblue)** for marketing/promotional campaigns:

- Booking confirmations sent instantly.
- New show notifications and reminders.
- Admin-triggered promotions to users.

---

## 🛠️ Tech Stack

| Technology  | Usage |
|:-------------|:----------|
| React.js      | Frontend Development |
| Node.js + Express.js | Backend APIs |
| MongoDB       | Database |
| Clerk         | Authentication |
| Stripe        | Payment Gateway |
| Ingest        | Transactional Emails |
| Brevo (Sendinblue) | Marketing & Reminder Emails |

---

## 🚀 Deployment — Vercel & Render

- **Frontend:** Deployed on **Vercel**
- **Backend:** Deployed on **Vercel**

---

## 🚀 Live Demo

🌐 Check it out here: [https://bookflix.vercel.app](https://book-flix-853w.vercel.app/)

---

## Getting Started

To get started with the Work Connect project, follow these steps:

1. Clone the repository from GitHub:

2. **Set Environment Variables**: Navigate to the `frontend` and `backend` folders and add necessary environment variables. You may need to create a `.env` file and configure it with required variables:
   In the backend/.env file:

   ```
   MONGODB_URI = your-mongodb-connection-uri
   CLERK_PUBLISHABLE_KEY = your-clerk-publishable-key
   CLERK_SECRET_KEY = your-clerk-secret-key  
   INNGEST_EVENT_KEY = your-inngest-event-key
   INNGEST_SIGNING_KEY = your-inngest-signing-key
   TMDB_API_KEY = your-tmdb-api-key 
   STRIPE_PUBLISHABLE_KEY = your-stripe-publishable-key
   STRIPE_SECRET_KEY = your-stripe-secret-key
   STRIPE_WEBHOOK_SECRET = your-stripe-webhook-secret 
   SENDER_EMAIL = your-sender-email
   SMTP_USER = your-smtp-user
   SMTP_PASS = your-smtp-password
   ```

   In the frontend/.env file:

   ```
   VITE_CLERK_PUBLISHABLE_KEY = your-publishable-key 
   VITE_CURRENCY = '$'
   VITE_BASE_URL = http://localhost:3000
   VITE_TMDB_IMAGE_BASE_URL = https://image.tmdb.org/t/p/original
   ```

3. **Install Dependencies**: Install dependencies in the `frontend` and `backend` folders using npm or yarn:

   ```
   cd frontend
   npm install
   cd ../backend
   npm install
   ```

4. **Start the Backend Server**: In the `backend` folder, start the development server using npm:

   ```
   npm run server
   ```

5. **Start the Frontend**: In the `frontend` folder, start the frontend application:

   ```
   npm run dev
   ```
