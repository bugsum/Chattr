# 💬 Chattr

**Chattr** is a lightweight real-time chat web app built with **Socket.IO**, **Express**, and modern frontend tech.  
Designed to be fast, minimal, and easy to scale — think of it as a DIY Slack-lite MVP.

---

## 🚀 Live URLs

| Type     | URL                                        |
|----------|--------------------------------------------|
| Frontend | [https://bugsum.github.io/chattr](https://bugsum.github.io/chattr) |
| Backend  | (coming soon)                              |

---

## 🧱 Monorepo Structure

```
/chattr
  /client     → Frontend (HTML/CSS/JS or React in future)
  /server     → Backend (Node.js + Express + Socket.IO)
  README.md   → You’re here
```

---

## ⚙️ Tech Stack

| Layer    | Tech                                      |
|----------|-------------------------------------------|
| Frontend | Vanilla JS (HTML/CSS), later React        |
| Backend  | Node.js + Express + Socket.IO             |
| Hosting  | GitHub Pages (frontend), Render/Railway (backend) |
| CI/CD    | GitHub Actions (for Pages deploy)         |
| Security | CORS, rate-limiting (planned)             |

---

## ✅ Features

### 📌 MVP Core

- [x] Real-time messaging with Socket.IO  
- [x] Multiple users connected in one room  
- [x] Message broadcasting + rendering  
- [ ] Unique usernames per session  
- [ ] Join/leave system messages  
- [ ] Typing indicators  
- [ ] Scrollback memory (in-memory or persistent)  
- [ ] Mobile-friendly UI  

### 🌟 Planned Features

- [ ] MongoDB message persistence  
- [ ] Private chat rooms  
- [ ] Auth via temporary token or username lock-in  
- [ ] Custom avatars or colors  
- [ ] Notification sounds or badges  
- [ ] `/commands` support (`/shrug`, `/me`, etc.)  

---

## 📝 Changelog

> A living feed of updates

### May 2025

- **[INIT]** Project scaffolded as monorepo  
- **[CORE]** Socket.IO basic connection and broadcast working  
- **[DEPLOY]** Frontend setup for GitHub Pages  
- **[DOCS]** Initial README created  

---

## 🛠️ Getting Started

### 🚧 Local Dev Setup

```bash
# Clone the repo
git clone https://github.com/bugsum/chattr.git
cd chattr

# Install dependencies
cd server && npm install
cd ../client && npm install # if you're using any bundler

# Start backend
cd server
node index.js

# Open client via Live Server or static server
cd ../client
open index.html # or use VSCode Live Server
```

> Make sure the Socket.IO client points to `localhost:3000` in dev.

---

## 🤖 GitHub Actions (Frontend Deploy)

A workflow is set up to:
- Build the frontend
- Push it to `gh-pages` branch
- Auto-deploy to `bugsum.github.io/chattr`

### Coming soon:
- Auto backend deploy to Render on push to `main`

---

## 🔐 Security Notes

To prevent abuse of the backend:
- [ ] CORS set to `bugsum.github.io`  
- [ ] Basic rate limiting middleware (planned)  
- [ ] Token auth (future enhancement)  

---

## 🙌 Contributions

> Not open to the public yet — but future-proofing this section.

Want to contribute? Open an issue or suggest a feature and fork the repo.

---

## 💡 About

Built by [@bugsum](https://github.com/bugsum) — just a dev building cool stuff.
