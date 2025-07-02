
# 🚀 Metaverse13 - Dockerized Next.js App

This is a production-ready, Dockerized Next.js application that uses server-side rendering (SSR). It is packaged with a multi-stage Dockerfile and deployable via GitHub.

---

## 📦 Features

- Built with [Next.js](https://nextjs.org/)
- Dockerized with multi-stage builds
- SSR and API routes supported
- Ready for deployment on any container-based platform

---

## 🛠️ Project Setup

### 1. Clone the Repo

```bash
git clone https://github.com/YOUR_USERNAME/metaverse13.git
cd metaverse13
```

### 2. Install Dependencies

```bash
npm install
```

---

## 🐳 Docker Setup

### 3. Build Docker Image

```bash
docker build -t my-react-app .
```

### 4. Run Docker Container

```bash
docker run -p 3000:3000 my-react-app
```

Open your browser at [http://localhost:3000](http://localhost:3000)

---

## 📁 File Structure

```
project/
├── pages/
├── public/
├── .next/              # Built output (ignored)
├── Dockerfile
├── .dockerignore
├── package.json
├── package-lock.json
└── README.md
```

---

## ⚙️ Deployment Notes

Ensure that your `package.json` includes:

```json
"scripts": {
  "dev": "next dev",
  "build": "next build",
  "start": "next start -H 0.0.0.0"
}
```

This makes sure the app is accessible from inside Docker.

---

## 📤 GitHub Deployment

```bash
git init
git remote add origin https://github.com/YOUR_USERNAME/metaverse13.git
git add .
git commit -m "Initial commit"
git push -u origin main
```

---

## ✅ License

MIT © 2025 Ismayil Mammadov
