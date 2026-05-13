# Portfolio — Adi Tata Koswara

Portfolio pribadi dibangun dengan **Astro** dan di-deploy ke **GitHub Pages**.

## 🚀 Cara Deploy ke GitHub Pages

### 1. Install dependencies
```bash
npm install
```

### 2. Coba jalankan lokal dulu
```bash
npm run dev
```
Buka http://localhost:4321

### 3. Push ke GitHub
```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/koswara198/portfolio.git
git push -u origin main
```

### 4. Aktifkan GitHub Pages
- Buka repo di GitHub
- Settings → Pages
- Source: pilih **"GitHub Actions"**
- Tunggu 1-2 menit → live di `https://koswara198.github.io/portfolio`

## ✏️ Cara Edit Konten

Semua konten ada di satu file: **`src/pages/index.astro`**

- **Tambah project baru** → edit array `projects` di bagian atas file
- **Update pengalaman kerja** → edit array `experience`
- **Tambah skill** → edit object `skills`

## 🏗️ Struktur Project
```
portfolio/
├── src/
│   ├── layouts/Layout.astro   # HTML head, fonts, global CSS
│   └── pages/index.astro      # Semua konten halaman
├── .github/
│   └── workflows/deploy.yml   # Auto-deploy ke GitHub Pages
├── astro.config.mjs
└── package.json
```
