# 🗓️ Google Calendar Clone  

A high-fidelity full-stack **Google Calendar Clone** built using **Next.js 14**, **Drizzle ORM**, and **PostgreSQL**.  
This project replicates the key features of Google Calendar — including event creation, editing, and deletion — with a clean and responsive user interface.

---

## 🚀 Features

✅ **Add, Edit & Delete Events** – Create and manage tasks directly from the calendar view.  
✅ **Month, Week & Day Views** – Switch between calendar views just like in Google Calendar.  
✅ **Interactive Popovers** – Add or modify events inline with smooth UI transitions.  
✅ **Persistent Storage** – All data is stored in a connected database using Drizzle ORM.  
✅ **Next.js App Router** – Modern routing with React Server Components.  
✅ **Real-time UI Refresh** – `revalidatePath()` ensures data stays synced between UI and DB.  
✅ **Responsive Design** – Works beautifully on both desktop and mobile.  

---

## 🧩 Tech Stack

| Layer | Technology |
|--------|-------------|
| **Frontend** | Next.js 14, React, Tailwind CSS |
| **State Management** | Zustand |
| **Backend** | Next.js Server Actions |
| **Database** | PostgreSQL + Drizzle ORM |
| **Styling** | Tailwind CSS + Shadcn/UI |
| **Icons** | Lucide Icons |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/google-calendar-clone.git
cd google-calendar-clone
```

### 2️⃣ Install Dependencies
```bash
npm install
```

### 3️⃣ Configure Environment Variables
Create a `.env.local` file in the root directory and add:
```env
DATABASE_URL="your_database_connection_url"
```

### 4️⃣ Apply Database Migrations
```bash
npx drizzle-kit push
```

### 5️⃣ Run the Development Server
```bash
npm run dev
```

Visit [http://localhost:3000](http://localhost:3000) to view your app.

---

## 🧠 Architecture Overview

- **Frontend (Client Side)** handles rendering the calendar grid, managing popovers, and displaying events interactively.
- **Backend (Server Actions)** performs CRUD operations (`createEvent`, `updateEvent`, `deleteEvent`) and revalidates data.
- **Database (Drizzle + PostgreSQL)** ensures data consistency and persistence.
- **State Management (Zustand)** stores UI states such as date selection, popover visibility, and event lists.

---

## 📁 Project Structure

```
📦 google-calendar-clone
├── app/                    # Next.js App Router
│   ├── page.tsx            # Main Calendar Page
│   ├── components/         # UI Components
│   └── actions/            # Server Actions (CRUD)
├── db/
│   ├── schema.ts           # Database Schema (Drizzle)
│   ├── drizzle.config.ts   # Drizzle Configuration
├── lib/
│   ├── store.ts            # Zustand Stores
│   └── utils.ts            # Helper Utilities
├── public/                 # Static Assets
└── README.md               # Documentation
```

---

## 💬 Known Limitations

- Authentication system is not yet implemented (all users share one calendar view).
- Recurring events are not supported in the current version.
- Week and day view toggles are planned for future releases.

---

## 🌟 Future Improvements

- Add **user authentication** with Clerk or NextAuth.  
- Implement **recurring and overlapping event logic**.  
- Integrate **Google Calendar API** for synchronization.  
- Add **drag-and-drop event rescheduling**.  
- Enhance animations using **Framer Motion**.

---

## 📜 License

This project is open-source and available under the **MIT License**.  
Feel free to fork, modify, and enhance it for your learning or projects.

---

## 👨‍💻 Author

**Developed by:** [Sahil Vashisth](https://github.com/sahilvashisth)  
**Inspired by:** Google Calendar’s clean UI & intuitive design.

---
