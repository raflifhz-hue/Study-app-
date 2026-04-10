# 📚 Study Desk

Aplikasi study planner dan catatan untuk pelajar. Dibuat dengan React + Vite.

## 🚀 Cara Menjalankan Lokal

```bash
# 1. Install dependencies
npm install

# 2. Jalankan development server
npm run dev

# 3. Buka browser di http://localhost:5173
```

## 📦 Build untuk Production

```bash
npm run build
```
Hasil build ada di folder `dist/`.

---

## 🌐 Deploy ke Vercel (Direkomendasikan)

### Cara 1 — Via GitHub (Termudah)

1. Push project ini ke GitHub:
   ```bash
   git init
   git add .
   git commit -m "first commit"
   git remote add origin https://github.com/USERNAME/study-desk.git
   git push -u origin main
   ```

2. Buka [vercel.com](https://vercel.com) → Login → **Add New Project**
3. Import repo dari GitHub
4. Klik **Deploy** — selesai! 🎉
5. Dapat URL seperti: `https://study-desk.vercel.app`

### Cara 2 — Via Vercel CLI

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel

# Ikuti instruksi di terminal
```

---

## 🌐 Deploy ke Netlify

### Cara 1 — Drag & Drop

```bash
npm run build
```
Lalu drag folder `dist/` ke [netlify.com/drop](https://app.netlify.com/drop)

### Cara 2 — Via CLI

```bash
npm install -g netlify-cli
npm run build
netlify deploy --prod --dir=dist
```

---

## 🌐 Deploy ke GitHub Pages

1. Tambahkan `"homepage"` di `package.json`:
   ```json
   "homepage": "https://USERNAME.github.io/study-desk"
   ```

2. Install gh-pages:
   ```bash
   npm install gh-pages --save-dev
   ```

3. Tambahkan scripts di `package.json`:
   ```json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d dist"
   ```

4. Deploy:
   ```bash
   npm run deploy
   ```

---

## 📁 Struktur Project

```
study-app/
├── public/
│   └── favicon.svg
├── src/
│   ├── App.jsx       ← Komponen utama
│   ├── index.css     ← Global styles
│   └── main.jsx      ← Entry point
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## ✨ Fitur

- 📋 **Study Plan** — tambah, edit, hapus, dan centang tugas
- 📝 **Notes** — catat materi per mata pelajaran
- 🏷️ Filter berdasarkan mata pelajaran
- 🔍 Pencarian catatan
- 📱 Mobile-friendly
