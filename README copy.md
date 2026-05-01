<div align="center">

```
 ██████╗██╗  ██╗ █████╗ ████████╗ ██████╗ ██████╗ ████████╗
██╔════╝██║  ██║██╔══██╗╚══██╔══╝██╔════╝ ██╔══██╗╚══██╔══╝
██║     ███████║███████║   ██║   ██║  ███╗██████╔╝   ██║   
██║     ██╔══██║██╔══██║   ██║   ██║   ██║██╔═══╝    ██║   
╚██████╗██║  ██║██║  ██║   ██║   ╚██████╔╝██║        ██║   
 ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝    ╚═════╝ ╚═╝        ╚═╝   
                    ✦ C L O N E ✦
```

### 🤖 A feature-rich, modern AI chatbot built with a powerful, type-safe full-stack

<br/>

![Next.js](https://img.shields.io/badge/Next.js_15-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white)

<br/>

![GitHub stars](https://img.shields.io/github/stars/kishan-ict/ChatGPT-Clone?style=flat-square&color=yellow)
![GitHub forks](https://img.shields.io/github/forks/kishan-ict/ChatGPT-Clone?style=flat-square&color=blue)
![GitHub issues](https://img.shields.io/github/issues/kishan-ict/ChatGPT-Clone?style=flat-square&color=red)
![License](https://img.shields.io/github/license/kishan-ict/ChatGPT-Clone?style=flat-square&color=green)

</div>

---

## 📌 Table of Contents

- [✨ Overview](#-overview)
- [🚀 Features](#-features)
- [🧱 Tech Stack](#-tech-stack)
- [🗂️ Project Structure](#️-project-structure)
- [⚙️ Getting Started](#️-getting-started)
- [🔐 Environment Variables](#-environment-variables)
- [🚢 Deployment](#-deployment)
- [🤝 Contributing](#-contributing)

---

## ✨ Overview

> **ChatGPT Clone** is a production-ready AI chat application that mirrors the experience of ChatGPT — built entirely from scratch using modern web technologies. Powered by **Google Gemini AI**, backed by **Supabase + Prisma**, and authenticated via **NextAuth**, this project goes beyond a basic clone to deliver a full-featured AI platform.

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│   User  ──►  Next.js App  ──►  Google Gemini API           │
│               │     │                  │                    │
│               ▼     ▼                  ▼                    │
│          NextAuth  Prisma ORM  ◄──  Supabase DB            │
│           (Auth)   (Queries)       (Postgres)               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## 🚀 Features

| Feature | Status |
|---|---|
| 🧠 AI Conversations powered by Google Gemini | ✅ Live |
| 💬 Real-time streaming responses | ✅ Live |
| 🔐 Secure Auth with NextAuth (Google OAuth) | ✅ Live |
| 🗂️ Persistent Chat History per user | ✅ Live |
| 📱 Fully Responsive UI (Mobile-first) | ✅ Live |
| 🌙 Dark / Light Mode Support | ✅ Live |
| 🗑️ Delete / manage conversations | ✅ Live |
| 🚀 One-click Vercel Deployment | ✅ Live |

---

## 🧱 Tech Stack

```
╔══════════════════════════════════════════════════════╗
║               ⚡ THE POWER STACK ⚡                  ║
╠═══════════════════╦══════════════════════════════════╣
║  LAYER            ║  TECHNOLOGY                      ║
╠═══════════════════╬══════════════════════════════════╣
║  Framework        ║  Next.js 15 (App Router)         ║
║  Language         ║  TypeScript                      ║
║  Styling          ║  Tailwind CSS                    ║
║  AI Provider      ║  Google Gemini API               ║
║  Auth             ║  NextAuth.js                     ║
║  ORM              ║  Prisma                          ║
║  Database         ║  Supabase (PostgreSQL)           ║
║  Deployment       ║  Vercel                          ║
╚═══════════════════╩══════════════════════════════════╝
```

### Why this stack?

- **Next.js 15** — App Router for server components, streaming, and edge-ready performance
- **Prisma + Supabase** — Type-safe database queries on a scalable, real-time Postgres backend
- **Google Gemini** — State-of-the-art AI with a generous free tier via AI Studio
- **NextAuth** — Plug-and-play auth with Google OAuth, zero headaches

---

## 🗂️ Project Structure

```
ChatGPT-Clone/
│
├── 📁 app/                    # Next.js App Router
│   ├── 📁 api/                # API Routes
│   │   ├── auth/              # NextAuth handler
│   │   └── chat/              # Gemini AI endpoint
│   ├── 📁 (auth)/             # Login / Register pages
│   └── 📁 chat/               # Main chat UI
│
├── 📁 components/             # Reusable UI components
│   ├── ChatMessage.tsx
│   ├── Sidebar.tsx
│   └── ...
│
├── 📁 lib/                    # Utilities & helpers
│   ├── prisma.ts              # Prisma client singleton
│   └── gemini.ts              # Gemini API wrapper
│
├── 📁 prisma/
│   └── schema.prisma          # Database schema
│
├── .env.local                 # 🔒 Your secrets (never commit!)
├── next.config.ts
└── package.json
```

---

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:

```bash
node --version   # v18+ required
npm --version    # or pnpm / yarn
```

You'll also need accounts on:
- [Supabase](https://supabase.com) — for your Postgres database
- [Google AI Studio](https://aistudio.google.com) — for the Gemini API key
- [Google Cloud Console](https://console.cloud.google.com) — for OAuth credentials

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/kishan-ict/ChatGPT-Clone.git
cd ChatGPT-Clone
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Configure Environment Variables

Create a `.env.local` file in the root directory:

```bash
cp .env.example .env.local   # if example exists, or create manually
```

Then fill in your values (see [Environment Variables](#-environment-variables) section below).

### 4️⃣ Push the Database Schema

```bash
npx prisma generate
npx prisma db push
```

### 5️⃣ Run the Development Server

```bash
npm run dev
```

Open **[http://localhost:3000](http://localhost:3000)** in your browser. 🎉

---

## 🔐 Environment Variables

Create a `.env.local` file in the project root and add the following:

```env
# ──────────────────────────────────────────────
# 🗄️  SUPABASE  (get from your project settings)
# ──────────────────────────────────────────────
DATABASE_URL="your_supabase_postgres_connection_string"
NEXT_PUBLIC_SUPABASE_URL="your_supabase_project_url"
NEXT_PUBLIC_SUPABASE_ANON_KEY="your_supabase_public_anon_key"

# ──────────────────────────────────────────────
# 🤖  GOOGLE AI  (get from AI Studio)
# ──────────────────────────────────────────────
GOOGLE_API_KEY="your_google_ai_studio_api_key"

# ──────────────────────────────────────────────
# 🔐  NEXTAUTH  (for authentication)
# ──────────────────────────────────────────────
NEXTAUTH_SECRET="generate_a_random_secret_string"
NEXTAUTH_URL="http://localhost:3000"

# For production, change NEXTAUTH_URL to your deployed URL
# NEXTAUTH_URL="https://your-app.vercel.app"
```

> 💡 **Tip:** Generate a secure `NEXTAUTH_SECRET` with:
> ```bash
> openssl rand -base64 32
> ```

### Where to get each key:

```
📍 Supabase keys  →  supabase.com → Your Project → Settings → API
📍 Google API key →  aistudio.google.com → Get API Key
📍 NextAuth URL   →  Your deployed domain (or localhost for dev)
```

---

## 🚢 Deployment

This project is optimized for **[Vercel](https://vercel.com)** — zero config needed.

```
1. Push your code to a GitHub repository
         │
         ▼
2. Go to vercel.com → Import Project → Select your repo
         │
         ▼
3. Add all .env.local variables to Vercel's Environment Settings
         │
         ▼
4. Click Deploy 🚀
         │
         ▼
5. Your app is LIVE! 🎉
```

> ⚠️ **Don't forget** to update `NEXTAUTH_URL` to your production Vercel URL before deploying.

---

## 📸 Screenshots

> _Add your own screenshots here to show off your UI!_
>
> ```markdown
> ![Chat UI](./public/screenshots/chat.png)
> ![Login Page](./public/screenshots/login.png)
> ```

---

## 🤝 Contributing

Contributions are welcome! Here's how to get involved:

```bash
# 1. Fork the repo on GitHub
# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/ChatGPT-Clone.git

# 3. Create a new branch
git checkout -b feature/your-amazing-feature

# 4. Make your changes and commit
git commit -m "feat: add your amazing feature"

# 5. Push to your branch
git push origin feature/your-amazing-feature

# 6. Open a Pull Request on GitHub 🎉
```

Please follow conventional commit messages: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

### Built with ❤️ by [kishan-ict](https://github.com/kishan-ict)

⭐ **If you found this project useful, please give it a star!** ⭐

[![GitHub stars](https://img.shields.io/github/stars/kishan-ict/ChatGPT-Clone?style=social)](https://github.com/kishan-ict/ChatGPT-Clone/stargazers)

</div>