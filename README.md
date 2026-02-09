<p align="center">
  <img src="client/public/icon.png" alt="Usaid Logo" width="200" />
</p>

# 🔮 Usaid - AI-Driven Cognitive Time Simulator

> **Experience the future before you choose it**

Usaid is an AI-powered decision-making tool that simulates multiple future timelines based on your life decisions. Using Google's Gemini AI, it generates personalized scenarios showing potential outcomes across emotional, financial, career, and relationship dimensions.

## ✨ Features

- **🧠 Multi-Timeline Generation** - Get 3-5 distinct future scenarios for any decision using Gemini 3 Flash
- **👤 Personalized Simulations** - AI considers your risk tolerance, priorities, and unique life situation
- **📊 Detailed Metrics** - Visualize emotional, financial, career, and relationship impacts
- **⚖️ Timeline Comparison** - Compare up to 3 timelines side-by-side to weigh trade-offs
- **🔄 Follow-up Decisions** - Inject new decisions to see how they alter futures dynamically
- **🔐 Secure Authentication** - Full sign-up/login flow with JWT security
- **🎨 Premium Experience** - Glassmorphism UI, Dark/Light mode, and immersive sound effects

## 📸 Screenshots

<!-- my screenshots will goes here -->
<div align="center">
  <img src="https://via.placeholder.com/800x450?text=Dashboard+Preview" alt="Dashboard Preview" width="800" />
</div>

## 🛠 Tech Stack

**Frontend:** React, TypeScript, Vite, Zustand, React Query, Glassmorphism UI  
**Backend:** Node.js, Express, Prisma (SQLite)  
**AI:** Google Gemini 3 API (Gemini 2.5 for fallback)

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- npm or yarn
- Gemini API key ([Get one here](https://aistudio.google.com/apikey))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ritikiitg/Usaid.git
   cd Usaid
   ```

2. **Setup the server**
   ```bash
   cd server
   npm install
   cp .env.example .env
   # Edit .env and add your GEMINI_API_KEY
   npx prisma migrate dev
   ```

3. **Setup the client**
   ```bash
   cd ../client
   npm install
   ```

### Running the Application

1. **Start the server** (from `/server`)
   ```bash
   npm run dev
   ```

2. **Start the client** (from `/client`)
   ```bash
   npm run dev
   ```

3. Open http://localhost:5173 in your browser

## 📁 Project Structure

```
usaid/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── stores/         # Zustand state stores
│   │   ├── services/       # API client
│   │   └── context/        # React contexts
│   └── public/             # Static assets
│
├── server/                 # Express backend
│   ├── src/
│   │   ├── routes/         # API routes
│   │   ├── services/       # Business logic
│   │   ├── middleware/     # Auth & error handling
│   │   └── lib/            # Prisma client
│   └── prisma/             # Database schema
│
└── README.md
```

## 🔑 Environment Variables

### Server (`/server/.env`)

| Variable | Description |
|----------|-------------|
| `PORT` | Server port (default: 3001) |
| `DATABASE_URL` | SQLite database path |
| `JWT_SECRET` | Secret for JWT tokens |
| `JWT_EXPIRES_IN` | Token expiration (e.g., 7d) |
| `GEMINI_API_KEY` | Your Gemini API key |

## 📝 License

Built for the Google DeepMind Hackathon 2026 by **Ritik Raj**

---

*Powered by Google Gemini*
