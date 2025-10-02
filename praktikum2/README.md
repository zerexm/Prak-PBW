# **FIARI AHMAD JULIANSYAH**

# **NPM:4523210048**



# 📌 Praktikum 2 - Aplikasi Pendaftaran Event (PHP)

## 📝 Deskripsi
Project ini merupakan aplikasi sederhana berbasis **PHP** yang digunakan untuk melakukan **pendaftaran event**.  
Pengguna dapat mengisi data diri berupa nama, email, dan tanggal lahir. Data yang berhasil divalidasi akan **disimpan ke file `pendaftar.txt`** dan ditampilkan dalam bentuk tabel daftar peserta.

---

## ⚙️ Fitur Utama
1. **Form Pendaftaran**
   - Input: Nama Lengkap, Email, dan Tanggal Lahir.
   - Validasi Email menggunakan **Regex**.
   - Validasi Tanggal Lahir (format **DD-MM-YYYY**) menggunakan **Regex**.

2. **Penyimpanan Data**
   - Data disimpan ke dalam file teks `pendaftar.txt` dengan format:
     ```
     Nama;Email;TanggalLahir
     ```

3. **Menampilkan Daftar Peserta**
   - Membaca isi file `pendaftar.txt`.
   - Menampilkan data dalam bentuk tabel di halaman web.

4. **Error Handling**
   - Menampilkan pesan error jika input tidak sesuai format.
   - Menampilkan pesan sukses jika pendaftaran berhasil.

---

## 🛠️ Konsep Pemrograman yang Digunakan
- **Constant** → `NAMA_EVENT`, `FILE_PENDAFTARAN`.
- **Variabel Global** → `$status_message`, `$error_messages`.
- **Fungsi dengan Regex**:
  - `validateEmail($email)`
  - `validateDate($date)`
- **Form Handling (POST Method)** → menangkap data dari form.
- **File Handling** → `file_put_contents()` untuk simpan data, `file()` untuk membaca data.
- **HTML + PHP** → integrasi front-end (form, tabel) dan back-end (logika PHP).

---

## ▶️ Cara Menjalankan
1. Pastikan sudah menginstal **XAMPP/Laragon** atau server PHP lain.
2. Simpan file sebagai `index.php`.
3. Letakkan file di folder `htdocs` (untuk XAMPP) atau folder server kamu.
4. Jalankan server Apache.
5. Akses melalui browser:
