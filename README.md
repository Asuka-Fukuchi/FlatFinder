# 🏠 FlatFinder

FlatFinder is a web application that connects property owners with renters.
Users can create, edit, delete, and favorite property listings, as well as send messages to property owners.

---

## 🛠 Skills

<strong>Frontend: </strong> Angular

<strong>Backend: </strong> Node.js, Express (developed by my teammate)

<strong>Database: </strong> MongoDB(chosen by teammate; originally planned as Firebase)

---

## 👥 Team Structure
Two-person collaborative project
- Teammate: Full backend + half of the frontend
- Me: Remaining half of frontend

---

## 💼 My Responsibilities (Frontend)
I was responsible for approximately half of the frontend development, including:
- Property creation, editing, and deletion pages
- User profile page (display & update)
- Favorites feature (add / remove / render on UI)
- Conditional UI behaviors such as:
   - Hiding the message section for a user’s own listings
   - Managing the favorites feature
- Refining my frontend implementation based on feedback to improve data consistency and usability

---
## 🔄 Project Context

The project was originally planned to use Firebase for simplicity, but the tech stack changed to MongoDB based on my teammate’s preference.
This resulted in a more complex backend design and required more careful coordination between frontend and backend.

I contributed by adjusting my frontend implementation to match the new API structure and worked closely with my teammate to ensure smooth integration.

---
## ✨ Features

- 🏠 View apartment listings with details
- 👤 Display landlord info (name, email)
- ⭐ Bookmark favorite flats
- 💬 Send & receive messages between users

---

## 🖼 Screenshots
### Home page
![Home Page](frontend/public/screenshots/home.png)
### Admin user's page
![Admin Page](frontend/public/screenshots/all-users.png)
### Flat Detail page
![Flat Detail](frontend/public/screenshots/flat-detail.png)

---

## 📂 Project Structure

```
flat-project/
├── backend/ # Backend (Node.js + Express + MongoDB)
│ ├── db/ # Database connection (connect.ts)
│ ├── models/ # Data models (flat, message, user)
│ └── routes/ # API routes (flat, message, user)
└── frontend/ # Frontend (Angular)
└── src/app/
├── components/ # Reusable UI components (header, footer)
├── pages/ # Page-level views (admin, auth, flat, home, my-page)
└── services/ # Angular services (auth, flat, message, user)
```

---

## 📦 Dependencies

### Frontend

- Angular CLI ^20.1.5
- Angular Compiler CLI ^20.1.0
- TypeScript ~5.8.2
- Karma / Jasmine (for testing)

### Backend

- Node.js (LTS)
- Express
- Mongoose
- dotenv
- cors
- jsonwebtoken
- bcrypt
- TypeScript ^5.9.2
- ts-node, nodemon (for development)

---

## 🚀 How to Run

1. Clone repository

   ```
   git clone https://github.com/username/flat-project.git
   cd flat-project
   ```

2. Install dependencies (both frontend & backend)

   ```
   cd frontend && npm install
   cd ../backend && npm install
   cd ..
   ```

3. Set environment variables <br>
   Create a .env file inside /backend:

   ```
   MONGO_URI=mongodb_connection_string
   PORT=3000
   JWT_SECRET=jwt_secret_key
   SECRET_ADMIN_KEY=SuperSecretAdmin2025
   ```

   ℹ️ If you want to register as an admin, just add ?adminkey=SuperSecretAdmin2025 to the register page URL. <br>
   Example: http://localhost:4200/register?adminkey=SuperSecretAdmin2025

4. Run the project (from root folder)

   ```
   npm run dev
   ```

   The dev script at the root will start both frontend (Angular) and backend (Express + Mongoose) simultaneously.

---

##  What I Learned

- How to collaborate in a environment where team members have different preferences and experience levels

- How to refine frontend code based on feedback to improve clarity and maintainability

- Improved ability to handle team-based workflows, communication, and Git collaboration

- Strengthened understanding of frontend–backend integration

