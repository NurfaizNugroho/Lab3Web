# Web1Lab3: Laporan Praktikum 3 - CSS Dasar

Repositori ini berisi hasil pengerjaan Praktikum 3 mata kuliah Pemrograman Web mengenai pengenalan dan penerapan *Cascading Style Sheets* (CSS) secara Internal, Eksternal, dan Inline CSS, serta penggunaan CSS Selector (ID dan Class Selector)[cite: 14].

## Data Mahasiswa
- **Nama:** Nurfaiz Pradibto Nugroho
- **NIM:** 312510172
- **Program Studi / Semester:** Teknik Informatika / 3
- **Kelas:** I253C
- **Mata Kuliah:** Pemrograman Web
- **Dosen Pengampu:** Agung Nugroho, S.Kom., M.Kom.
- **Hari / Tanggal:** Sabtu, 10 Oktober 2026 (Pertemuan 4 - Offline)
- **Instansi:** Universitas Pelita Bangsa

---

## Langkah-langkah Praktikum

Berikut adalah alur pengerjaan Praktikum 3 beserta rincian struktur kode dan tampilannya:

### 1. Persiapan dan Struktur Dasar HTML
- Mempersiapkan text editor (Visual Studio Code).
- Membuat folder kerja baru dengan nama `praktikum-3-css-dasar`.
- Membuat file baru dengan nama `lab2_css_dasar.html` yang berisi kerangka navigasi, kontainer `#intro`, heading, paragraf teks, serta tombol tautan dengan class `.button .btn-primary`.

![Struktur HTML Dasar](/praktikum-3-css-dasar/images/img-1.jpg)
![Tampilan Awal HTML](/praktikum-3-css-dasar/images/img-2.jpg)

### 2. Implementasi CSS Internal
- Menambahkan tag `<style>` di dalam bagian `<head>` dokumen untuk mendeklarasikan CSS secara internal.
- Mengatur properti styling untuk tag `body`, `header`, `h1`, serta styling khusus tag anak `h1 i`.

![Kode CSS Internal](/praktikum-3-css-dasar/images/img-3.jpg)
![Tampilan CSS Internal](/praktikum-3-css-dasar/images/img-4.jpg)

### 3. Implementasi Inline CSS
- Menambahkan atribut `style` (`style="text-align: center; color: #ccd8e4;"`) secara langsung pada elemen paragraf untuk mengatur perataan teks dan warna secara spesifik.

![Kode Inline CSS](/praktikum-3-css-dasar/images/img-5.jpg)
![Tampilan Inline CSS](/praktikum-3-css-dasar/images/img-6.jpg)

### 4. Implementasi CSS Eksternal
- Membuat file terpisah bernama `style_eksternal.css` untuk mengatur gaya navigasi (`nav`, `nav a`, `nav .active`, dan `nav a:hover`).
- Menyisipkan file CSS eksternal ke dalam dokumen HTML menggunakan tag `<link>` pada bagian `<head>`.

![Kode CSS Eksternal](/praktikum-3-css-dasar/images/img-7.jpg)
![Tag Link CSS Eksternal](/praktikum-3-css-dasar/images/img-8.jpg)
![Tampilan CSS Eksternal](/praktikum-3-css-dasar/images/img-9.jpg)

### 5. Penambahan ID Selector dan Class Selector
- Menambahkan aturan styling untuk Class Selector (`.button` dan `.btn-primary`) pada file `style_eksternal.css` untuk memperindah tampilan tombol interaktif.

![Kode ID & Class Selector](/praktikum-3-css-dasar/images/img-10.jpg)
![Tampilan Akhir Praktikum](/praktikum-3-css-dasar/images/img-11.jpg)

---

## Pertanyaan dan Tugas

### 1. Eksperimen Properti CSS
Melakukan eksperimen dengan mengubah dan menambah properti serta nilai pada kode CSS mengacu pada *CSS Cheat Sheet*, seperti penerapan gradasi (`linear-gradient`), sudut melengkung (`border-radius`), bayangan (`box-shadow`), serta efek interaktif transisi (`hover` dan `translateY`) pada elemen navigasi, kontainer `#intro`, dan tombol.

### 2. Perbedaan `h1 {...}` dengan `#intro h1 {...}`
- **`h1 {...}` (Element/Tag Selector):** Berfungsi untuk menargetkan seluruh elemen `h1` di seluruh dokumen HTML secara global.
- **`#intro h1 {...}` (Descendant Selector):** Berfungsi secara spesifik untuk menargetkan elemen `h1` yang hanya berada di dalam kontainer ber-ID `intro` dengan tingkat spesifisitas yang lebih tinggi.

### 3. Prioritas Deklarasi CSS (Internal, Eksternal, dan Inline)
- **Deklarasi yang Ditampilkan:** **Inline CSS**.
- **Penjelasan:** Dalam aturan kaskade CSS (*Cascading Order*), urutan prioritas dari yang terendah ke tertinggi adalah **CSS Eksternal $\rightarrow$ CSS Internal $\rightarrow$ Inline CSS**. Karena ditulis langsung pada atribut elemen HTML, Inline CSS memiliki kekuatan tertinggi yang menimpa seluruh aturan gaya lainnya.

### 4. Prioritas CSS antara ID dan Class Selector pada Elemen yang Sama
- **Deklarasi yang Ditampilkan:** **ID Selector**.
- **Penjelasan:** Berdasarkan sistem spesifisitas CSS (*CSS Specificity*), ID Selector (`#id`) memiliki bobot dan prioritas yang jauh lebih tinggi dibandingkan Class Selector (`.class`). Oleh karena itu, jika terjadi konflik properti pada elemen yang sama, aturan pada ID akan lebih diutamakan oleh browser.