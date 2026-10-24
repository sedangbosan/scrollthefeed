---
title: "Style Guide"
pubDate: 2026-10-24
description: "Panduan visual untuk elemen tipografi dan konten Markdown."
---

Artikel ini berfungsi sebagai referensi untuk melihat bagaimana berbagai elemen Markdown ditampilkan pada blog. Gunakan halaman ini untuk mengevaluasi tipografi, jarak antar-elemen, keterbacaan, dan konsistensi desain.

## Heading

Heading digunakan untuk membagi tulisan menjadi bagian-bagian yang mudah dipindai.

### Heading level 3

Gunakan subheading ketika sebuah bagian membutuhkan pembagian topik yang lebih spesifik.

#### Heading level 4

Heading level 4 cocok untuk struktur yang lebih mendalam. Hindari penggunaan heading hanya untuk memperbesar teks.

## Paragraf

Ini adalah contoh paragraf standar. Panjang baris, tinggi baris, dan jarak antarparagraf berpengaruh besar terhadap kenyamanan membaca. Pada layar lebar maupun perangkat seluler, teks sebaiknya tetap memiliki lebar yang terkendali agar pembaca tidak kehilangan jejak saat berpindah dari satu baris ke baris berikutnya.

Paragraf kedua menguji jarak vertikal antara blok teks. Desain yang baik tidak harus ramai atau dekoratif. Tipografi yang konsisten, kontras yang memadai, dan ruang kosong yang proporsional sudah cukup untuk menciptakan pengalaman membaca yang nyaman.

Teks dapat menggunakan **bold untuk penekanan**, *italic untuk istilah atau nuansa tertentu*, maupun ~~strikethrough untuk teks yang tidak lagi berlaku~~.

## Tautan

Tautan dapat digunakan di dalam kalimat, misalnya mengunjungi [dokumentasi Astro](https://docs.astro.build/) atau membaca [panduan Markdown](https://www.markdownguide.org/).

Tautan sebaiknya mudah dikenali tanpa mengganggu alur membaca.

## Blockquote

> Desain yang baik bukan hanya tentang apa yang terlihat, tetapi juga tentang bagaimana sesuatu digunakan dan dirasakan.

Kutipan dapat digunakan untuk menonjolkan pendapat, catatan, atau pernyataan penting dari sumber lain.

## Daftar

### Unordered list

- Kesederhanaan dalam desain.
- Konsistensi dalam tipografi.
- Performa yang baik di berbagai perangkat.
  - Ukuran layar desktop.
  - Ukuran layar seluler.
- Aksesibilitas bagi semua pembaca.

### Ordered list

1. Tentukan tujuan tulisan.
2. Susun struktur konten.
3. Tulis dan edit isi artikel.
4. Periksa tampilan di berbagai ukuran layar.

### Task list

- [x] Menentukan struktur artikel.
- [x] Menulis konten contoh.
- [ ] Memeriksa kontras warna.
- [ ] Menguji tampilan pada perangkat seluler.

## Tabel

| Elemen | Kegunaan | Prioritas |
| --- | --- | --- |
| Heading | Membentuk hierarki konten | Tinggi |
| Paragraf | Menyampaikan informasi | Tinggi |
| Tautan | Menghubungkan sumber | Sedang |
| Blockquote | Menonjolkan kutipan | Sedang |
| Tabel | Membandingkan data | Sesuai kebutuhan |

Tabel sebaiknya tetap mudah dibaca di layar kecil. Jika diperlukan, gunakan pembungkus dengan horizontal scrolling.

## Gambar

Tambahkan gambar dengan teks alternatif yang menjelaskan isi atau fungsi gambar tersebut.

![Contoh ilustrasi lanskap pegunungan dan danau](https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=1200&q=80)

*Contoh caption untuk gambar. Caption sebaiknya singkat dan memberikan konteks tambahan.*

## Inline code

Gunakan `inline code` untuk menyebut nama variabel, fungsi, perintah, atau istilah teknis di dalam kalimat.

Contohnya, file konfigurasi Astro biasanya menggunakan `astro.config.mjs`, sedangkan konten Markdown dapat disimpan di `src/content/blog/`.

## Code block

Contoh konfigurasi sederhana:

```js
const site = {
  title: "My Personal Blog",
  description: "Catatan tentang teknologi dan kehidupan.",
  theme: "system",
};

console.log(site.title);
```

Contoh perintah terminal:

```bash
npm install
npm run dev
npm run build
```

Blok kode yang baik harus memiliki jarak yang cukup, mudah dibaca, dan memungkinkan teks panjang digulir secara horizontal jika diperlukan.

## Elemen tambahan

Gunakan garis pemisah untuk memisahkan dua bagian yang memiliki hubungan tetapi membutuhkan batas visual.

---

Teks kecil seperti nama file, tanggal, dan keterangan tambahan sebaiknya tetap memiliki kontras yang memadai terhadap latar belakang.

## Penutup

Style guide ini dapat digunakan sebagai halaman uji ketika mengubah warna, font, ukuran teks, jarak, atau komponen artikel. Setelah desain diperbarui, periksa kembali halaman ini untuk memastikan semua elemen tetap konsisten dalam mode terang maupun gelap, serta di desktop dan perangkat seluler.
