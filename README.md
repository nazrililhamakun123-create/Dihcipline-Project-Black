# DIHCIPLINE — Progressive Web App (PWA)

Ini versi PWA dari aplikasi stickman-mu. Bedanya dengan APK: **tidak perlu
build apa-apa** — cukup di-hosting sebagai file statis di internet (harus
HTTPS), lalu dibuka lewat browser HP, dan browser akan menawarkan tombol
**"Install app" / "Tambahkan ke Layar Utama"** — hasilnya jadi ikon di HP
seperti aplikasi biasa, bisa dibuka tanpa browser bar, dan tetap bisa dipakai
offline berkat service worker.

## Isi folder
- `index.html` — aplikasi stickman (sudah ditambah tag PWA)
- `manifest.json` — identitas aplikasi (nama, ikon, warna)
- `service-worker.js` — bikin aplikasi bisa jalan offline
- `icons/` — ikon aplikasi (192px, 512px, dan versi maskable)

## Cara hosting (pilih salah satu)

### Opsi A — GitHub Pages (gratis, cocok karena kamu sudah punya repo)
1. Buat repository baru di GitHub (atau pakai repo `dihcipline-app` yang sudah ada).
2. Upload **semua isi folder ini** ke root repo tersebut (drag & drop lewat
   "uploading an existing file" di GitHub, sama seperti sebelumnya).
3. Buka **Settings → Pages** di repo itu.
4. Di bagian **Source**, pilih branch `main` dan folder `/ (root)` → Save.
5. Tunggu 1–2 menit, GitHub akan memberi URL seperti:
   `https://<username>.github.io/<nama-repo>/`
6. Buka URL itu di Chrome HP Android kamu.

### Opsi B — Netlify Drop (paling cepat, tanpa akun/git)
1. Buka **app.netlify.com/drop** di komputer.
2. Seret seluruh folder ini ke halaman tersebut.
3. Netlify langsung memberi URL publik siap pakai.

## Cara install ke HP
1. Buka URL hosting-nya di **Chrome** (Android).
2. Ketuk menu titik tiga → **"Tambahkan ke Layar utama"** / **"Install app"**
   (kadang muncul otomatis sebagai banner di bawah).
3. Ikon "DIHCIPLINE" akan muncul di home screen HP, terbuka fullscreen tanpa
   address bar, dan tetap bisa dibuka walau tanpa internet setelah pertama
   kali dibuka.

## Catatan
- PWA **wajib** diakses lewat HTTPS agar bisa diinstal (GitHub Pages dan
  Netlify sudah otomatis HTTPS).
- Untuk mengganti tampilan, edit `index.html` lalu upload ulang / push ulang.
