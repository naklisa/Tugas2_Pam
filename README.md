# Dokumen Tugas Pemrograman Web - Website Semantik ITERA

**Nama**: Nahli Saud Ramdani <br>
**NIM**: 123140049 <br>
**Nama Proyek**: Website Sederhana Institut Teknologi Sumatera (ITERA) <br>
**Tipe Tugas**: HTML Only (Penggunaan Struktur Semantik HTML5) <br>
**File Utama**: `index.html`, `berita.html`, `DOKUMENTASI.md`

---

## 1. Alasan Pemilihan Struktur Semantik HTML

Struktur semantik HTML5 digunakan untuk memberikan makna logis (*meaning*) pada setiap bagian elemen web, tidak hanya untuk tampilan visual, melainkan juga untuk aksesibilitas (*accessibility*) dan optimasi mesin pencari (*SEO*).

Berikut adalah alasan penggunaan setiap tag semantik dalam proyek ini:

1. **`<header>`**:
   - **Lokasi**: Bagian atas halaman `index.html` dan `berita.html`.
   - **Alasan**: Digunakan untuk menampung identitas utama situs, seperti logo ITERA (`<img>`), nama perguruan tinggi (`<h1>`), serta slogan/tagline kampus.
2. **`<nav>`**:
   - **Lokasi**: Di bawah header pada kedua halaman.
   - **Alasan**: Membungkus daftar tautan navigasi utama (`<ul>` & `<li>`) yang menghubungkan antarhalaman (`index.html` dan `berita.html`) serta *anchor links* ke bagian internal halaman.
3. **`<main>`**:
   - **Lokasi**: Bagian tengah pembungkus utama konten.
   - **Alasan**: Menandai area konten yang unik dan paling penting dari halaman tersebut, membedakannya dari header, navigasi, dan footer yang bersifat berulang.
4. **`<section>`**:
   - **Lokasi**: Di dalam `<main>`, membungkus profil kampus, data statistik, inovasi, dan kumpulan berita.
   - **Alasan**: Mengelompokkan konten-konten berdasarkan topik atau tema pembahasan secara terstruktur. Setiap `<section>` dilengkapi dengan judul heading (`<h2>` - `<h4>`).
5. **`<table>`**:
   - **Lokasi**: Pada `<section id="statistik">` di `index.html`.
   - **Alasan**: Menyajikan data kuantitatif civitas akademika ITERA (jumlah mahasiswa, dosen, tendik, dan skor SINTA) secara teratur dan mudah dibaca oleh pembaca layar (*screen reader*). Dibuat lengkap dengan elemen semantik `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, `<th>`, `<tr>`, dan `<td>`.
6. **`<article>`**:
   - **Lokasi**: Pada bagian inovasi di `index.html` dan artikel berita di `berita.html`.
   - **Alasan**: Membungkus konten independen yang dapat berdiri sendiri dan didistribusikan ulang (seperti publikasi riset dan berita kegiatan kampus).
7. **`<aside>`**:
   - **Lokasi**: Di samping/bawah konten utama pada kedua halaman.
   - **Alasan**: Menampung informasi pelengkap atau sekunder yang berkaitan dengan konten utama, seperti pengumuman PMB, tautan layanan cepat, dan pilihan kategori berita.
8. **`<footer>`**:
   - **Lokasi**: Bagian paling bawah setiap halaman.
   - **Alasan**: Menampilkan catatan kaki, informasi alamat kampus (`<address>`), dan hak cipta (*copyright*).
9. **Heading Terstruktur (`<h1>` s.d. `<h6>`)**:
   - **Alasan**: Diterapkan dengan hirarki yang ketat dan tidak melompati level (misalnya `<h1>` untuk judul halaman utama, `<h2>` untuk seksi utama, `<h3>` untuk sub-seksi, hingga `<h6>` untuk catatan detail) guna menjamin kejelasan struktur dokumen.

---

## 2. Tantangan dan Solusi

Selama pengerjaan tugas HTML-only ini, terdapat beberapa tantangan teknis yang dihadapi beserta solusinya:

| No | Tantangan Teknis | Solusi yang Diterapkan |
|---|---|---|
| 1 | **Menjaga keterbacaan tampilan tanpa CSS (HTML-Only)** | Mengatur hierarki elemen secara logis, memanfaatkan pembatas baris (`<hr>`), daftar terstruktur (`<ul>`, `<ol>`), serta atribut gaya tabel (`style="border: 1px solid black;"`) agar tampilan tetap rapi dan lolos W3C Validator. |
| 2 | **Memastikan Hirarki Heading Terstruktur (`h1`-`h6`)** | Merancang hierarki heading secara teliti pada artikel berita di `berita.html`, di mana `<h1>` digunakan untuk judul portal berita, `<h2>` untuk bagian seksi berita, `<h3>` untuk artikel utama, `<h4>` untuk latar belakang, `<h5>` untuk spesifikasi daya, dan `<h6>` untuk catatan uji coba. |
| 3 | **Kepatuhan Kriteria W3C Validator** | Menggunakan penutupan tag yang konsisten, menambahkan atribut wajib seperti `alt` pada `<img>`, `lang="id"` pada `<html>`, meta `charset="UTF-8"`, serta menghindari tag non-standar yang dapat memicu *warning* atau *error*. |

---
