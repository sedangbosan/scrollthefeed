---
title: "Membangun blog yang cepat tanpa mengorbankan kenyamanan membaca"
description: "Beberapa prinsip sederhana untuk membuat situs konten terasa ringan, fokus, dan nyaman dibaca."
pubDate: 2026-10-24
category: "Web & Performance"
tags: ["Astro", "Performance", "Writing"]
draft: false
---

Blog yang baik tidak perlu banyak bergerak untuk terasa hidup. Yang paling penting adalah tulisan mudah ditemukan, nyaman dibaca, dan halaman tidak membuat pembaca menunggu.

## Mulai dari konten

Gunakan judul yang deskriptif, paragraf yang tidak terlalu panjang, dan heading yang membantu pembaca memindai tulisan. Satu paragraf idealnya membahas satu gagasan utama.

## Kurangi kerja browser

Untuk blog berbasis konten, HTML statis sering kali sudah cukup. Hindari JavaScript di sisi klien jika fitur tersebut tidak benar-benar membutuhkan interaksi.

```css
.article {
  max-width: 70ch;
  margin-inline: auto;
  line-height: 1.85;
}
```

## Jadikan Markdown sebagai sumber tulisan

Setiap artikel disimpan sebagai berkas `.md`. Frontmatter berisi metadata, sementara isi artikel tetap Markdown standar.

> Desain yang baik bukan sekadar dekorasi; desain membantu pembaca memberi perhatian pada hal yang penting.

## Checklist sebelum publish

- Periksa judul dan deskripsi halaman.
- Gunakan gambar yang terkompresi jika memang diperlukan.
- Pastikan kontras teks cukup tinggi.
- Uji tampilan di ponsel dan keyboard.
- Jalankan build produksi sebelum deploy.
