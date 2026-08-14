# KargoOke — Website

Source code website KargoOke. Statis, tanpa build step.

## Menjalankan

Semua halaman bisa dibuka langsung dari browser (double click file `.html`). Untuk menjalankan lewat server lokal:

```bash
python3 -m http.server 8080
```

Lalu buka `http://localhost:8080`.

## Struktur

| File | Halaman |
|---|---|
| `index.html` | Beranda |
| `OkeComply.html` | Produk — OkeComply |
| `OkeShip.html` | Produk — OkeShip |
| `OkePort.html` | Produk — OkePort |
| `OkeDebit.html` | Produk — OkeDebit |
| `OkeData.html` | Produk — OkeData |
| `OkeBiz.html` | Produk — OkeBiz |
| `TentangKami.html` | Tentang Kami |
| `demo-gratis.html` | Form demo gratis |
| `registration.html` | Form registrasi |
| `registration-success.html` | Halaman sukses registrasi |
| `assets/` | Logo dan gambar |

## Catatan teknis

- Setiap halaman **self-contained**: CSS dan JavaScript ditulis inline di dalam file HTML masing-masing, jadi tidak ada dependency antar file selain `assets/`.
- Font diambil dari Google Fonts, jadi halaman butuh koneksi internet untuk tampil dengan tipografi yang benar.
- Sebagian gambar contoh masih memakai layanan placeholder (`images.unsplash.com`, `i.pravatar.cc`). Ganti dengan aset final sebelum production.
- Belum ada backend: form registrasi dan demo gratis masih berupa tampilan, submit-nya perlu disambungkan ke endpoint.

## Deploy

Cukup unggah seluruh isi folder ini ke web server atau static hosting (Netlify, Vercel, GitHub Pages, atau hosting biasa). Tidak perlu proses build.
