# 🏫 SMP Mentari — Website Informasi Sekolah

<p align="center">
  <strong>Aplikasi Website Sekolah Berbasis Laravel</strong><br>
  Praktikum Pemrograman Berbasis Web — Pertemuan 5
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.2%2B-777BB4?logo=php&logoColor=white" alt="PHP 8.2+">
  <img src="https://img.shields.io/badge/Laravel-12-FF2D20?logo=laravel&logoColor=white" alt="Laravel 12">
  <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?logo=tailwindcss&logoColor=white" alt="Tailwind CSS v4">
  <img src="https://img.shields.io/badge/Project-Praktikum-blue" alt="Project Praktikum">
</p>
---

## 📋 Identitas Mahasiswa

| Keterangan | Informasi |
|---|---|
| Nama | Ridwan Odi Nugroho |
| NPM | 4524210089 |
| Program Studi | Teknik Informatika |
| Universitas | Universitas Pancasila |
| Mata Kuliah | Pemrograman Berbasis Web |
| Praktikum | Pertemuan 5 |

## 📖 Deskripsi Proyek

**SMP Mentari** merupakan aplikasi website informasi sekolah yang dikembangkan menggunakan framework Laravel. Proyek ini dibuat sebagai bagian dari praktikum Pemrograman Berbasis Web untuk mempelajari pengembangan aplikasi web dinamis, pengelolaan data, autentikasi pengguna, dan konfigurasi aplikasi.

Aplikasi dirancang untuk menyediakan halaman informasi sekolah, menampilkan kegiatan sekolah, menerima pesan dari pengunjung, serta menyediakan fitur pengelolaan data melalui operasi CRUD (*Create, Read, Update, Delete*).

Proyek ini juga menerapkan pengaturan dinamis agar beberapa perilaku aplikasi dapat dikonfigurasi tanpa harus mengubah langsung kode pada setiap halaman. Sistem autentikasi digunakan untuk mendukung pembatasan akses terhadap halaman tertentu.

## 🎯 Tujuan Praktikum

Tujuan pengembangan aplikasi SMP Mentari adalah:

1. Memahami penggunaan Laravel dalam membangun website dinamis.
2. Menerapkan konsep routing, controller, model, dan view.
3. Membuat proses pengelolaan data menggunakan operasi CRUD.
4. Mengintegrasikan basis data dengan aplikasi web.
5. Menerapkan autentikasi pengguna menggunakan Laravel Breeze.
6. Memahami pembatasan akses halaman menggunakan middleware.
7. Membuat pengaturan aplikasi yang dapat diubah secara dinamis.
8. Menggunakan Blade Template untuk menyusun tampilan halaman.
9. Mengelola aset frontend menggunakan Tailwind CSS dan Vite.
10. Melakukan pengujian terhadap fungsi aplikasi.

## ✨ Fitur Utama

### 1. 🏠 Halaman Utama

Halaman utama menjadi bagian awal website SMP Mentari. Halaman ini digunakan untuk menampilkan informasi yang berkaitan dengan sekolah serta menyediakan navigasi menuju bagian website lainnya.

### 2. 📅 Informasi Kegiatan Sekolah

Fitur kegiatan sekolah digunakan untuk mengelola informasi kegiatan yang ditampilkan pada website.

Pengelolaan data kegiatan dapat melibatkan operasi CRUD sesuai implementasi aplikasi:

- **Create:** Menambahkan informasi kegiatan.
- **Read:** Menampilkan daftar dan informasi kegiatan.
- **Update:** Memperbarui informasi kegiatan.
- **Delete:** Menghapus data kegiatan.

### 3. 💬 Pesan Tamu

Fitur pesan tamu menyediakan sarana bagi pengunjung untuk mengirimkan pesan melalui website.

Data pesan dapat dikelola melalui sistem agar informasi yang dikirimkan dapat disimpan dan ditampilkan sesuai alur aplikasi.

### 4. ⚙️ Pengaturan Dinamis

Aplikasi menggunakan pengaturan untuk mengatur perilaku tertentu pada halaman website.

Salah satu pengaturan yang digunakan dalam proyek adalah:

`home_kegiatan_per_page`

Pengaturan tersebut digunakan untuk menentukan jumlah kegiatan yang ditampilkan pada halaman utama. Nilai yang digunakan pada konfigurasi awal proyek adalah `6`.

Dengan pengaturan ini, jumlah kegiatan yang ditampilkan dapat disesuaikan melalui konfigurasi aplikasi tanpa perlu menuliskan angka yang sama secara berulang di berbagai bagian kode.

### 5. 🔐 Autentikasi Pengguna

Aplikasi menggunakan Laravel Breeze sebagai dasar sistem autentikasi.

Fitur autentikasi membantu mengatur proses masuk pengguna dan akses menuju halaman yang memerlukan login.

Penggunaan middleware juga membantu memastikan bahwa halaman tertentu tidak dapat diakses oleh pengguna yang belum memenuhi persyaratan autentikasi.

### 6. 📊 Dashboard

Dashboard merupakan halaman untuk mengakses fitur pengelolaan aplikasi setelah pengguna berhasil login, sesuai aturan akses yang diterapkan.

Dashboard membantu memisahkan halaman yang ditujukan kepada pengunjung umum dengan bagian aplikasi yang digunakan untuk pengelolaan data.

## 🛠️ Teknologi yang Digunakan

| Teknologi | Fungsi |
|---|---|
| PHP 8.2+ | Bahasa pemrograman backend |
| Laravel 12 | Framework pengembangan aplikasi web |
| Laravel Breeze | Dasar autentikasi pengguna |
| Blade Template | Menampilkan halaman dinamis |
| Tailwind CSS v4 | Mengatur tampilan dan desain antarmuka |
| Vite | Menjalankan dan membangun aset frontend |
| MySQL atau SQLite | Basis data sesuai konfigurasi proyek |
| Composer | Mengelola dependensi PHP |
| Node.js dan npm | Mengelola dependensi frontend |
| Git dan GitHub | Pengelolaan versi dan penyimpanan kode |

## 🧠 Konsep Pemrograman yang Diterapkan

### 1. Routing

Routing digunakan untuk menentukan alamat URL dan proses yang dijalankan ketika pengguna membuka halaman tertentu.

Pada Laravel, definisi route website umumnya diletakkan dalam:

`routes/web.php`

Route dapat mengarahkan permintaan menuju controller atau langsung menampilkan view, sesuai kebutuhan aplikasi.

### 2. Model dan Basis Data

Model digunakan untuk merepresentasikan data aplikasi dan membantu interaksi dengan basis data melalui Eloquent ORM.

Pada SMP Mentari, konsep ini digunakan untuk mendukung pengelolaan data seperti kegiatan sekolah dan pesan tamu.

### 3. Controller

Controller menangani proses yang berhubungan dengan permintaan pengguna. Controller dapat menerima input, menjalankan validasi, memanggil model, dan mengembalikan hasil kepada halaman.

Pemisahan proses ke dalam controller membantu menjaga kode agar lebih terstruktur.

### 4. Blade Template

Blade merupakan template engine Laravel yang digunakan untuk membuat halaman dinamis.

Dengan Blade, tampilan dapat disusun menggunakan HTML dan dilengkapi data yang dikirim dari controller.

Contoh sederhana:

```blade
<h1>Selamat Datang di SMP Mentari</h1>

<p>Website Informasi Sekolah</p>
```

Contoh tersebut hanya menggambarkan penggunaan Blade dan bukan salinan keseluruhan halaman proyek.

### 5. CRUD

CRUD merupakan konsep dasar pengelolaan data yang terdiri atas empat operasi:

| Operasi | Penjelasan |
|---|---|
| Create | Menambahkan data baru |
| Read | Membaca atau menampilkan data |
| Update | Mengubah data yang tersedia |
| Delete | Menghapus data |

Penerapan CRUD membantu memahami bagaimana data dimasukkan melalui formulir, diproses oleh aplikasi, disimpan dalam basis data, dan ditampilkan kembali kepada pengguna.

### 6. Autentikasi dan Middleware

Laravel Breeze menyediakan dasar autentikasi yang membantu pengelolaan proses login dan fitur akun pengguna.

Middleware digunakan untuk memeriksa kondisi tertentu sebelum sebuah permintaan diproses lebih lanjut, misalnya memastikan pengguna sudah login sebelum membuka halaman dashboard.

### 7. Pengaturan Dinamis

Pengaturan dinamis memungkinkan nilai tertentu dikelola melalui konfigurasi atau mekanisme pengaturan aplikasi.

Contohnya, jumlah kegiatan yang ditampilkan pada halaman utama menggunakan nilai `home_kegiatan_per_page`. Pendekatan ini membantu mengurangi ketergantungan pada nilai tetap yang ditulis langsung di banyak tempat.

## 🔄 Alur Kerja Aplikasi

Secara umum, alur penggunaan website dapat digambarkan sebagai berikut:

```text
              Pengunjung Website
                     |
                     v
               Halaman Utama
                     |
          +----------+----------+
          |                     |
          v                     v
    Informasi Sekolah       Pesan Tamu
          |
          v
   Informasi Kegiatan

---------------------------------------

           Pengguna Terautentikasi
                     |
                     v
                   Login
                     |
                     v
              Pemeriksaan Akses
                     |
                     v
                 Dashboard
                     |
          +----------+----------+
          |                     |
          v                     v
   Kelola Kegiatan        Kelola Pesan
          |                     |
          +----------+----------+
                     |
                     v
              Proses CRUD
                     |
                     v
                 Basis Data
```

Diagram tersebut merupakan gambaran konseptual alur aplikasi. Alur aktual mengikuti route, controller, middleware, dan hak akses yang diterapkan pada kode proyek.

## 📂 Struktur Proyek

Berikut gambaran struktur umum proyek Laravel SMP Mentari. Struktur sebenarnya dapat berbeda bergantung pada berkas yang tersedia dalam repository.

```text
SMP-Mentari/
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   └── Middleware/
│   ├── Models/
│   └── Providers/
├── bootstrap/
├── config/
├── database/
│   ├── migrations/
│   ├── factories/
│   └── seeders/
├── public/
├── resources/
│   ├── css/
│   ├── js/
│   └── views/
├── routes/
│   ├── web.php
│   └── auth.php
├── storage/
├── tests/
├── .env.example
├── artisan
├── composer.json
├── package.json
└── vite.config.js
```

### Penjelasan Bagian Penting

| Direktori atau Berkas | Kegunaan |
|---|---|
| `app/Http/Controllers/` | Menangani proses permintaan pengguna |
| `app/Models/` | Merepresentasikan data dan interaksi dengan basis data |
| `resources/views/` | Menyimpan halaman Blade |
| `resources/css/` | Menyimpan kode CSS frontend |
| `resources/js/` | Menyimpan kode JavaScript frontend |
| `routes/web.php` | Mendefinisikan route website |
| `routes/auth.php` | Route autentikasi jika tersedia |
| `database/migrations/` | Mendefinisikan struktur tabel |
| `database/seeders/` | Menyediakan data awal jika digunakan |
| `config/` | Menyimpan konfigurasi aplikasi |
| `public/` | Menyimpan aset publik |
| `tests/` | Menyimpan pengujian otomatis |
| `.env` | Menyimpan konfigurasi lingkungan lokal |
| `composer.json` | Mendefinisikan dependensi PHP |
| `package.json` | Mendefinisikan dependensi frontend |

## 💻 Persyaratan Sistem

Sebelum menjalankan aplikasi, pastikan perangkat telah memiliki:

- PHP 8.2 atau versi lebih baru.
- Composer.
- Node.js dan npm.
- MySQL atau SQLite, sesuai konfigurasi basis data.
- Browser modern.
- Git, apabila ingin melakukan clone repository.

XAMPP dapat digunakan untuk menyediakan lingkungan pengembangan lokal, khususnya jika proyek dikonfigurasi menggunakan MySQL.

## 🚀 Instalasi dan Konfigurasi

### 1. Clone Repository

Clone repository utama:

```bash
git clone https://github.com/RidwanOdi/4524210089_RIDWANODINUGROHO_PBW-A.git
```

Masuk ke folder Praktikum 5:

```bash
cd "4524210089_RIDWANODINUGROHO_PBW-A/Praktikum 5/SMP-Mentari"
```

Jika repository sudah diunduh, langsung buka terminal pada direktori `SMP-Mentari`.

### 2. Instal Dependensi PHP

Jalankan:

```bash
composer install
```

Perintah tersebut memasang paket PHP yang dibutuhkan berdasarkan `composer.json`.

### 3. Instal Dependensi Frontend

Jalankan:

```bash
npm install
```

Perintah ini memasang dependensi frontend yang didefinisikan dalam `package.json`.

### 4. Siapkan File Environment

Jika `.env` belum tersedia, salin file contoh menggunakan PowerShell:

```powershell
Copy-Item .env.example .env
```

Kemudian jalankan:

```bash
php artisan key:generate
```

Jangan menimpa file `.env` yang sudah berisi konfigurasi lokal penting tanpa membuat salinan terlebih dahulu.

### 5. Konfigurasi Basis Data

Sesuaikan konfigurasi `.env` dengan basis data yang digunakan oleh proyek.

Contoh konfigurasi MySQL:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=smp_mentari
DB_USERNAME=root
DB_PASSWORD=
```

Nama database dan kredensial di atas adalah contoh. Sesuaikan dengan konfigurasi lokal.

Jika proyek menggunakan SQLite, gunakan konfigurasi SQLite yang sesuai dengan lingkungan proyek, bukan konfigurasi MySQL di atas.

### 6. Jalankan Migration

Setelah konfigurasi database benar, jalankan:

```bash
php artisan migrate
```

Migration digunakan untuk membuat atau memperbarui struktur tabel berdasarkan file migration yang tersedia.

**Perhatian:** Hindari menjalankan perintah reset database pada lingkungan yang menyimpan data penting karena perintah tersebut dapat menghapus data.

### 7. Jalankan Aplikasi

Untuk menjalankan server Laravel:

```bash
php artisan serve
```

Untuk menjalankan frontend selama pengembangan, buka terminal kedua dan jalankan:

```bash
npm run dev
```

Buka browser dan kunjungi:

`http://127.0.0.1:8000`

Jika ingin membangun aset frontend untuk penggunaan tanpa development server Vite, jalankan:

```bash
npm run build
```

## 🧪 Pengujian Aplikasi

Proyek menyediakan perintah pengujian yang dapat dijalankan melalui Composer:

```bash
composer test
```

Perintah ini digunakan untuk menjalankan test script yang didefinisikan pada `composer.json`.

### Skenario Pengujian

| No. | Skenario | Hasil yang Diharapkan |
|---|---|---|
| 1 | Membuka halaman utama | Halaman utama ditampilkan |
| 2 | Membuka informasi kegiatan | Data kegiatan ditampilkan sesuai implementasi |
| 3 | Mengirim pesan tamu | Pesan diproses sesuai aturan aplikasi |
| 4 | Login dengan data valid | Pengguna dapat login |
| 5 | Login dengan data tidak valid | Sistem menolak data yang salah |
| 6 | Membuka dashboard tanpa login | Akses dibatasi sesuai middleware |
| 7 | Menambahkan data kegiatan | Data dapat disimpan jika fitur tersedia |
| 8 | Mengubah data kegiatan | Perubahan dapat disimpan jika fitur tersedia |
| 9 | Menghapus data kegiatan | Data dapat dihapus jika fitur tersedia |
| 10 | Mengubah pengaturan jumlah kegiatan | Tampilan mengikuti nilai pengaturan |
| 11 | Logout | Sesi pengguna berakhir |

Tabel tersebut merupakan rencana pengujian, bukan bukti bahwa seluruh skenario telah berhasil. Hasil aktual perlu diperiksa ketika aplikasi dijalankan.

## 🛡️ Keamanan dan Pengelolaan Konfigurasi

Beberapa hal yang perlu diperhatikan dalam pengembangan dan pengumpulan proyek:

- Jangan mengunggah file `.env` yang berisi kredensial atau kunci aplikasi.
- Gunakan `.env.example` untuk mendokumentasikan konfigurasi yang diperlukan tanpa menyertakan rahasia.
- Pastikan input pengguna divalidasi sebelum diproses.
- Batasi akses ke halaman pengelolaan data sesuai autentikasi dan otorisasi aplikasi.
- Jangan menyimpan dependensi hasil instalasi seperti `vendor/` dan `node_modules/` ke repository apabila direktori tersebut memang dikecualikan oleh `.gitignore`.
- Periksa konfigurasi database sebelum menjalankan migration.
- Jalankan pengujian setelah perubahan kode untuk memastikan fitur tetap berfungsi.

## 🔧 Penanganan Masalah

### Composer tidak dikenali

Pastikan Composer sudah terinstal dan tersedia pada `PATH`. Periksa dengan:

```bash
composer --version
```

### PHP tidak dikenali

Periksa instalasi PHP dan konfigurasi `PATH`:

```bash
php --version
```

### Database tidak terhubung

Periksa apakah layanan database aktif, nama database benar, dan konfigurasi `.env` sesuai. Setelah memperbaiki konfigurasi Laravel, jalankan:

```bash
php artisan config:clear
```

### Migration gagal

Periksa koneksi database, status tabel, dan pesan error dari Laravel. Pastikan database yang dipilih memang tersedia.

### Tampilan frontend tidak muncul dengan benar

Pastikan dependensi frontend terpasang dan jalankan:

```bash
npm install
npm run dev
```

### Dashboard tidak dapat dibuka

Periksa status login dan middleware pada route dashboard. Pastikan akun telah memenuhi persyaratan akses yang diterapkan.

## 🚀 Pengembangan Selanjutnya

Aplikasi SMP Mentari dapat dikembangkan lebih lanjut melalui beberapa peningkatan berikut:

1. **Pencarian kegiatan sekolah** agar pengguna lebih mudah menemukan informasi.
2. **Pagination kegiatan** untuk mengelola tampilan ketika jumlah data semakin banyak.
3. **Pengelolaan kategori kegiatan** agar informasi lebih terorganisasi.
4. **Validasi pesan tamu** untuk membantu menjaga kualitas data yang diterima.
5. **Peningkatan dashboard** dengan ringkasan informasi yang relevan.
6. **Pengaturan website tambahan** untuk mendukung konfigurasi konten.
7. **Pengujian otomatis tambahan** untuk route, autentikasi, dan operasi CRUD.
8. **Peningkatan desain responsif** agar website nyaman digunakan pada berbagai ukuran layar.
9. **Peningkatan aksesibilitas** untuk membantu pengguna mengakses konten.
10. **Deployment** agar aplikasi dapat diakses melalui server daring.

Daftar tersebut merupakan usulan pengembangan, bukan klaim bahwa seluruh fitur telah diimplementasikan.

## 📌 Kesimpulan

Praktikum 5 melalui proyek SMP Mentari memberikan pengalaman dalam membangun aplikasi website menggunakan Laravel. Proyek ini menggabungkan konsep routing, controller, model, Blade Template, autentikasi, pengelolaan data, dan pengaturan dinamis.

Penggunaan operasi CRUD membantu memahami proses pengelolaan data dari input hingga penyimpanan dan penampilan kembali. Sementara itu, Laravel Breeze dan middleware memberikan dasar untuk mengatur autentikasi dan akses halaman.

Melalui praktikum ini, mahasiswa diharapkan dapat memahami struktur aplikasi Laravel dan menerapkan konsep pengembangan web secara lebih terorganisasi, serta mampu melakukan pengujian dan pengembangan fitur sesuai kebutuhan.

---

<p align="center">
  <strong>Ridwan Odi Nugroho</strong><br>
  4524210089<br>
  Teknik Informatika — Universitas Pancasila<br><br>
  <em>Praktikum Pemrograman Berbasis Web — Pertemuan 5</em>
</p>
