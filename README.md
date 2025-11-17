# lab8-praktikum-web
# Nama : Sheila Antica Oktaviani
# Kelas : TI.24.A1
# NIM : 312410002
# Dosen : Agung Nugroho, S.Kom., M.Kom.
# Mata Kuliah : Pemograman Web
## 1. koneksi.php
File ini berfungsi untuk menghubungkan aplikasi PHP ke database MySQL.
## Penjelasan fungsi file:
1. Menyimpan informasi server database (nama host, username, password, nama database).
2. Membuat koneksi agar file lain bisa mengambil, menambah, mengubah, atau menghapus data dari database.
3. Jika koneksi gagal, biasanya akan muncul pesan error.
## 2. tambah.php
File ini digunakan untuk menambah data barang baru ke dalam database.
## Penjelasan prosesnya:
- Menampilkan form input (seperti nama barang, harga, stok, foto).
- User mengisi form dan mengirim data.
- Data yang dikirim akan diproses:
- Dicek apakah sudah terisi lengkap.
-Jika ada foto, foto akan di-upload ke folder tertentu.
- Jika semua valid, data akan disimpan ke tabel barang di database.
- Setelah berhasil, user akan diarahkan kembali ke halaman utama (misal ke index.php).
## 3. ubah.php
File ini digunakan untuk mengedit data barang yang sudah ada.
Penjelasan prosesnya:
- Mengambil data barang berdasarkan ID barang yang ingin diubah.
- Menampilkan form yang sudah berisi data lama agar bisa diedit.
- User mengganti data sesuai kebutuhan.
- Sistem memperbarui data di database:
- Jika foto tidak diganti, foto lama tetap dipakai.
- Jika foto diganti, sistem akan upload foto baru dan menghapus foto lama.
- Setelah berhasil, sistem akan kembali ke halaman utama.
## 4. style.css 
style
File ini berisi pengaturan tampilan (desain) pada semua halaman.
Penjelasan fungsinya:
Mengatur ukuran teks, jenis font, margin, dan jarak halaman.
Mengatur tampilan tabel seperti garis, warna header, jarak kolom.
Mengatur ukuran gambar agar rapi. Mengatur tampilan form input seperti ukuran kotak teks, tombol submit, warna tombol, dan efek hover.
Mengatur layout container supaya posisi konten berada di tengah halaman.
## Penjelasan INDEX.PHP
index.php biasanya berfungsi sebagai halaman utama yang menampilkan seluruh data dari database.
Di halaman ini:
1. Menampilkan Data
index.php akan mengambil semua data dari database menggunakan query seperti SELECT.
Data tersebut ditampilkan dalam bentuk tabel (misalnya daftar buku, daftar produk, daftar pengguna).
2. Tombol Aksi (Edit & Hapus)
Pada setiap baris data, biasanya ada tombol:
Edit → menuju halaman edit.php
Hapus → menuju hapus.php?id=…
Jadi index.php berfungsi sebagai pusat semua daftar data.
3. Link Tambah Data
Biasanya ada tombol Tambah Data, untuk masuk ke halaman tambah.php.
4. Menghubungkan ke Database
index.php akan melakukan koneksi ke database untuk mengambil data dan menampilkannya.
## Penjelasan HAPUS.PHP
hapus.php digunakan untuk menghapus data berdasarkan ID.
Cara kerjanya:
1. Menerima ID
hapus.php menerima parameter seperti:
hapus.php?id=5
ID tersebut menunjukkan data mana yang akan dihapus.
2. Menjalankan Query Delete
hapus.php menjalankan perintah SQL:
DELETE FROM nama_tabel WHERE id = ...
Setelah query berhasil, data di database akan hilang.
3. Mengembalikan ke index.php
Setelah selesai menghapus, biasanya diarahkan kembali ke index.php agar daftar data diperbarui.
# Input 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/21e67264-5d33-4460-853e-2226b1056645" />

# Input data_barang
<img width="1278" height="1824" alt="carbon (15)" src="https://github.com/user-attachments/assets/90f927b3-1e49-409a-be40-17b63b40bbc6" />

# Hasil di Web data_barang
<img width="956" height="353" alt="image" src="https://github.com/user-attachments/assets/aed34905-46e3-4ae2-8a4b-aba5cde98ee5" />

# Input Tambah Barang

<img width="1296" height="2122" alt="carbon (16)" src="https://github.com/user-attachments/assets/a497440f-0377-41bf-8c5c-bb250f583b64" />

# Hasil di Web Tambah barang
<img width="598" height="358" alt="image" src="https://github.com/user-attachments/assets/de993c7b-7691-446a-94ff-6bb3e07248ea" />

# Input Ubah
<img width="1548" height="4096" alt="carbon (18)" src="https://github.com/user-attachments/assets/f5575dac-2697-4cd5-8923-63774279620e" />

# Hasil Web Ubah Barang
<img width="959" height="323" alt="image" src="https://github.com/user-attachments/assets/a0490195-df73-4fa7-83a8-87e4f4f4330e" />




