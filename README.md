# Vibe Coding Challenge — Sistem Penilaian

Web app untuk lomba Vibe Coding syukuran angkatan.
Peserta submit karya, panitia nilai, leaderboard otomatis.

---

## Cara Deploy (ikutin urutan ini)

### Step 1 — Buat Project Firebase

1. Buka https://console.firebase.google.com
2. Klik "Add project" → kasih nama (contoh: `vibe-coding-angkatan`)
3. Disable Google Analytics → klik "Create project"
4. Tunggu sampai selesai → klik "Continue"

### Step 2 — Aktifkan Firestore Database

1. Di sidebar kiri, klik **Build** → **Firestore Database**
2. Klik "Create database"
3. Pilih **"Start in test mode"** → klik Next
4. Pilih region **asia-southeast1 (Singapore)** → klik Enable
5. Tunggu sampai database aktif

### Step 3 — Ambil Firebase Config

1. Klik ikon ⚙️ (Project Settings) di sidebar kiri
2. Scroll ke bawah ke bagian **"Your apps"**
3. Klik ikon **`</>`** (Web)
4. Isi App nickname (bebas) → klik "Register app"
5. Copy seluruh isi `firebaseConfig` yang muncul

### Step 4 — Tempel Config ke Kode

Buka file `index.html`, cari bagian ini (sekitar baris 220):

```javascript
const firebaseConfig = {
  apiKey: "GANTI_API_KEY",
  authDomain: "GANTI_PROJECT.firebaseapp.com",
  projectId: "GANTI_PROJECT_ID",
  ...
};
```

Ganti dengan config yang lo copy tadi.

### Step 5 — Upload ke GitHub

1. Buat akun GitHub kalau belum ada: https://github.com
2. Klik "New repository" → kasih nama → Create
3. Upload semua file di folder ini (index.html, vercel.json, README.md)
   - Bisa lewat tombol "Add file → Upload files" di GitHub

### Step 6 — Deploy ke Vercel

1. Buka https://vercel.com → Sign up dengan akun GitHub
2. Klik "Add New → Project"
3. Import repository yang tadi lo buat
4. Klik **Deploy** (tanpa ubah apapun)
5. Selesai! Lo dapet URL seperti: `https://vibe-coding-angkatan.vercel.app`

---

## Cara Pakai Saat Lomba

| Tab | Siapa | Fungsi |
|-----|-------|--------|
| Submit Karya | Peserta | Isi data + link karya |
| Dashboard Panitia | Lo (PJ) | Nilai semua peserta |
| Leaderboard | Semua | Lihat ranking final |
| Panduan | Lo (PJ) | Referensi hari H |

## Rubrik Penilaian

| Kriteria | Skor |
|----------|------|
| Fungsionalitas (app jalan & sesuai tema) | 0–50 |
| Kreativitas (ide unik & bermanfaat) | 0–30 |
| Efektivitas AI (prompt terarah & iteratif) | 0–20 |
| **Total** | **100** |

---

Dibuat untuk Syukuran Angkatan — Lomba Vibe Coding
