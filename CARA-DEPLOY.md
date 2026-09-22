# Cara Deploy Website GASPOL ke GitHub Pages (Gratis)

File `index.html` di folder ini adalah seluruh website kamu — satu file, tidak perlu instalasi apapun.

## Langkah-langkah

1. **Buat akun GitHub** (kalau belum punya) di https://github.com/signup

2. **Buat repository baru**
   - Klik tombol "+" di kanan atas → "New repository"
   - Nama repository bebas, contoh: `gaspol-website`
   - Pilih "Public"
   - Klik "Create repository"

3. **Upload file `index.html`**
   - Di halaman repository yang baru dibuat, klik "uploading an existing file"
   - Seret file `index.html` ke area upload
   - Klik "Commit changes"

4. **Aktifkan GitHub Pages**
   - Buka tab "Settings" di repository tersebut
   - Di menu kiri, klik "Pages"
   - Di bagian "Branch", pilih `main` dan folder `/ (root)`
   - Klik "Save"

5. **Tunggu 1-2 menit**, lalu website kamu akan aktif di alamat:
   `https://<username-github-kamu>.github.io/<nama-repository>/`

   Contoh: `https://budi123.github.io/gaspol-website/`

## Kalau nanti mau pakai domain sendiri (misal gaspolmotor.id)

1. Beli domain di penyedia seperti Niagahoster, Domainesia, atau Namecheap
2. Di pengaturan DNS domain, arahkan (CNAME) ke `<username-github-kamu>.github.io`
3. Di GitHub Pages Settings, masukkan domain itu di kolom "Custom domain"

## Catatan tentang forum & form gabung

Form pendaftaran anggota sekarang meneruskan isian langsung ke WhatsApp admin.
Nomornya diatur lewat variabel `ADMIN_WA` di dalam `index.html` (cari baris
`var ADMIN_WA`). Tulis dalam format internasional tanpa tanda "+", misal nomor
08123456789 ditulis 628123456789. Setiap pendaftaran akan masuk sebagai chat
WhatsApp ke nomor itu.

Forum masih menyimpan obrolan di browser masing-masing pengunjung, jadi topik
yang ditulis satu orang belum terlihat oleh pengunjung lain. Ini cukup untuk
pratinjau. Kalau mau forum benar-benar jalan bersama, perlu ditambahkan backend
(bisa dibahas terpisah kalau sudah siap ke tahap itu).
