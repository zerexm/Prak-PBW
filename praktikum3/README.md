# **FIARI AHMAD JULIANSYAH**

# **NPM:4523210048**



# 📌 Praktikum 3 - LARAPRESS aplikasi blog sederhana

## 📝 Deskripsi
LaraPress adalah aplikasi blog sederhana yang dibangun menggunakan Laravel 12 untuk tujuan pembelajaran dan pengembangan keterampilan web development

---

## ⚙️ **Tentang Proyek**
Proyek ini dibuat sebagai bagian dari pembelajaran Laravel framework. LaraPress mendemonstrasikan konsep-konsep dasar Laravel seperti routing, views, dan struktur MVC.

**Fitur yang Sudah Diimplementasikan**
   - Data disimpan ke dalam file teks `pendaftar.txt` dengan format:
     ```
     Nama;Email;TanggalLahir
     ```

1. **Halaman Utama (Welcome Page)**
  - Mengubah tampilan default Laravel menjadi halaman sederhana
  - Menampilkan judul "Selamat Datang di LaraPress"
  - Struktur HTML yang bersih dan minimal.

2. **Halaman Tentang Kami**
   - Route: /tentang-kami
   - Menampilkan informasi tentang LaraPress
   - Menjelaskan tujuan proyek sebagai pembelajaran Laravel 12

## 📁 Struktur File yang Dimodifikasi
- **resources/views/welcome.blade.php**  
  Mengubah tampilan default Laravel menjadi HTML sederhana dan menampilkan pesan sambutan.  

- **resources/views/about.blade.php (baru)**  
  File view baru untuk halaman "Tentang Kami".  

- **routes/web.php**  
  Menambahkan route `/tentang-kami` yang mengarah ke view `about.blade.php`.

---

## 🛠️ Langkah Implementasi

### Step 1: Modifikasi Halaman Welcome
File: `resources/views/welcome.blade.php`
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Selamat Datang di LaraPress</title>
</head>
<body>
  <h1>Selamat Datang di Blog LaraPress</h1>
  <p>Ini adalah halaman utama dari aplikasi blog kita.</p>
</body>
</html>

### Step 2: Membuat Route Baru

Tambahkan route baru pada file routes/web.php:

Route::get('/tentang-kami', function () {
    return view('about');
});

### Step 3: Membuat View About

Buat file baru resources/views/about.blade.php:

<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tentang Kami - LaraPress</title>
</head>
<body>
  <h1>Tentang LaraPress</h1>
  <p>LaraPress adalah aplikasi blog sederhana yang dibuat dengan Laravel 12.</p>
  <p>Proyek ini dibuat untuk tujuan pembelajaran dan pengembangan keterampilan.</p>
</body>
</html>

## 🌐 Endpoint yang Tersedia
Route	Method	Deskripsi
/	GET	Halaman utama LaraPress
/tentang-kami	GET	Halaman tentang LaraPress
## 💻 Teknologi yang Digunakan

Framework: Laravel 12

PHP Version: 8.x

Database: SQLite (default)

Frontend: Blade Template Engine, HTML, CSS

Build Tool: Vite

## 📦 Instalasi
Step 1: Clone Repository
git clone https://github.com/adiwp/pbw.git
cd pro1

### Step 2: Install Dependencies
composer install
npm install

### Step 3: Setup File Environment
cp .env.example .env

### Step 4: Generate Application Key
php artisan key:generate

### Step 5: Jalankan Development Server
php artisan serve

### Step 6: Akses Aplikasi

Buka browser lalu masuk ke:
👉 http://localhost:8000

##📸 Screenshot
Halaman Utama

Halaman Tentang Kami

## 🔄 Git History

Seluruh perubahan sudah di-commit dan di-push dengan pesan commit yang jelas untuk setiap modifikasi.

## 📝 Rencana Pengembangan

 Menambahkan sistem autentikasi

 Membuat fitur CRUD untuk artikel blog

 Menambahkan sistem komentar

 Implementasi kategori dan tag

 Membuat dashboard admin

 Menambahkan styling dengan Tailwind CSS

 Implementasi fitur pencarian

## 👨‍💻 Pengembang

Nama: Adi Wahyu

Repository: pbw

Branch: main

## 📄 Lisensi

Proyek ini menggunakan lisensi MIT - lihat file LICENSE
 untuk detail lebih lanjut.

## 📜 Catatan

Proyek ini dibuat untuk tujuan pembelajaran.
Silakan lakukan fork dan modifikasi sesuai kebutuhan Anda!

## 🤝 Kontribusi

Dalam rangka memastikan komunitas Laravel tetap ramah untuk semua, harap patuhi Code of Conduct.

## 🔐 Keamanan

Jika menemukan kerentanan keamanan dalam Laravel, segera hubungi fiariahmad di fiariahmad@laravel.com
. Semua masalah keamanan akan segera ditangani.
