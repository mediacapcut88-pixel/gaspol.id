# Website GASPOL — Cara Rilis & Memperbarui

File `index.html` di folder ini adalah seluruh website — satu file, tidak perlu instalasi apapun.

## Website sudah rilis

Alamatnya: **https://mediacapcut88-pixel.github.io/gaspol.id/**

Repo: https://github.com/mediacapcut88-pixel/gaspol.id

Langkah manual di bawah ini sudah dikerjakan semua, jadi tidak perlu diulang.
Catatan ini disimpan kalau nanti perlu bikin website kedua.

## Cara memperbarui website

Setelah mengubah `index.html`, jalankan tiga perintah ini di folder WEBSITE:

```
git add -A
git commit -m "jelaskan perubahannya di sini"
git push
```

Website akan ikut berubah sekitar 1-2 menit kemudian. Tidak perlu upload
manual lagi lewat browser.

Kalau lebih nyaman lewat browser: buka repo di GitHub, klik file `index.html`,
klik ikon pensil, edit, lalu "Commit changes".

## Langkah manual (arsip, kalau mau bikin website lain)

1. **Buat repository baru** di https://github.com/new, pilih "Public"

2. **Upload file `index.html`** lewat tautan "uploading an existing file"

3. **Aktifkan GitHub Pages** di Settings -> Pages -> Branch: `main`, folder `/ (root)` -> Save

4. **Tunggu 1-2 menit**, website aktif di
   `https://<username-github-kamu>.github.io/<nama-repository>/`

## Kalau nanti mau pakai domain sendiri (misal gaspolmotor.id)

1. Beli domain di penyedia seperti Niagahoster, Domainesia, atau Namecheap
2. Di pengaturan DNS domain, arahkan (CNAME) ke `mediacapcut88-pixel.github.io`
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
