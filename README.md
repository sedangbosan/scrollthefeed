# Scroll the Feed — Astro blog template

Template blog minimalis untuk Astro, Markdown, dan Cloudflare Pages. Tanpa sidebar, tanpa font eksternal, dan tanpa JavaScript client-side untuk UI inti.

## Fitur

- Halaman daftar tulisan dan halaman artikel dari Markdown.
- Content collection dengan validasi frontmatter.
- Responsif, layout single-column, lebar baca sekitar 70 karakter.
- System font stack, tanpa request Google Fonts.
- Light/dark theme mengikuti preferensi sistem.
- Metadata title, description, canonical, serta `robots.txt`.
- Header keamanan dasar untuk Cloudflare Pages.
- Draft tidak ditampilkan di build publik.

## Menjalankan lokal

```bash
npm install
npm run dev
```

Buka URL lokal yang ditampilkan Astro.

## Menulis artikel

Buat file baru di `src/content/blog/nama-artikel.md`:

```md
---
title: "Judul artikel"
description: "Ringkasan singkat untuk daftar artikel dan mesin pencari."
pubDate: 2026-10-24
category: "Catatan"
tags: ["Astro", "Web"]
draft: false
---

Isi artikel dengan Markdown.
```

Frontmatter `title`, `description`, dan `pubDate` wajib diisi. `category`, `tags`, dan `draft` memiliki nilai default. Gunakan `draft: true` untuk mengecualikan tulisan dari build.

## Deploy ke Cloudflare Pages

1. Push folder proyek ini ke repository GitHub/GitLab.
2. Di Cloudflare Dashboard, buka **Workers & Pages → Create → Pages → Connect to Git**.
3. Pilih repository.
4. Isi pengaturan build:
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
5. Simpan dan deploy. Setiap push ke branch produksi akan memicu build baru.

Untuk deploy CLI, instal Wrangler dan jalankan `npm run build`, lalu `npx wrangler pages deploy dist`.

## Kustomisasi desain

Variabel warna berada di awal CSS global dalam `src/layouts/BaseLayout.astro`:
- `--bg`: warna latar
- `--text`: warna teks
- `--muted`: teks sekunder
- `--line`: garis pemisah
- `--accent`: aksen ungu
- `--accent-soft`: latar label kategori

Palet ini terinspirasi nuansa netral dan ungu pada antarmuka Zen Browser, bukan salinan resmi token warna mereka. Dark mode otomatis mengikuti preferensi OS.

## Catatan performa

- Astro menghasilkan halaman statis saat build.
- Tidak ada framework UI, script analitik, font remote, atau gambar hero yang otomatis diunduh.
- Hindari menambahkan library besar jika CSS dan HTML sudah mencukupi.
- Skor PageSpeed aktual tetap bergantung pada hosting, konten, gambar, dan konfigurasi tambahan.
