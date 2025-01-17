# Aplikasi Double-Entry Bookkeeping Bakwan

Software akuntansi simple yang dibuat dengan bahasa pemrograman [Singkong](https://github.com/nopri/nopri.github.io).

## Daftar Isi

1. [Apa itu _*Double-Entry Bookkeeping*_ ?](#apa-itu-double-entry-bookkeeping)
2. [Links](#links)
3. [Tahapan Development](#tahapan-development)
4. [Panduan Penggunaan Aplikasi](#panduan-penggunaan-aplikasi)
5. [Referensi](#referensi)

## Apa itu _*Double-Entry Bookkeeping*_ ?

**_Double-entry bookkeeping_** bisa juga disebut sebagai sistem pembukuan ganda atau tata buku berpasangan. Double-entry bookkeeping adalah sistem pencatatan seluruh transaksi ke dalam dua aspek, yaitu debit dan kredit yang orientasinya selalu dalam keadaan seimbang. Debit ditulis di kiri dan kredit di kanan.

Dalam _double-entry bookkeeping_, setiap transaksi akan dicatat dalam dua akun, yaitu di akun debit dan akun kredit. Contohnya, jika sebuah perusahaan meminjam uang sebesar Rp 3.000.000, maka di bagian debit akan ada akun kas sebesar Rp 3.000.000 dan di bagian kredit akan ada akun utang sebesar Rp 3.000.000. Debit dan kredit harus seimbang. _Double-entry bookkeeping_ juga berpegang pada rumus aset sama dengan utang ditambah ekuitas.

## Links

- Bahasa Pemrograman Singkong : https://nopri.github.io/Singkong.jar
- Aplikasi Double-Entry Bookkeeping Bakwan : https://github.com/nopri/bakwan

## Tahapan Development

- Update 1.0 (30 Oktober 2023)

  - Menggunakan **Singkong** Versi 8.3.
  - Dapat memasukkan Nama Perusahaan dan Tanggal Fiskal.

- Update 1.2 (08 November 2023)

  - Penambahan fitur template sederhana untuk Chart Of Accounts dan Tabelnya.
  - Menambahkan tombol "New", "Edit", dan "Delete" yang belum berfungsi.

- Update 1.3 (11 November 2023)

  - Menggunakan **Singkong** Versi 8.4.
  - Perubahan Syling pada datepicker agar lebih seragam dengan tombol lain.
  - Draft dialog new account pada Chart Of Account, yang didadalm akun tersebut terdapat tipe akun, kode akun, dan deskripsi.

- Update 1.4 (12 November 2023)

  - Penyesuaian nama Variabel untuk mnemonic
  - Usulan kode akun sesuai tipe akun baru
  - Tombol "Reset"

- Update 1.5 (13 November 2023)

  - Menggunakan **Singkong** Versi 8.5.
  - Alignment Kode akun sesuai tipe akun baru.

- Update 1.6 (17 November 2023)

  - Penambahan dialog pada tombol "New", "Edit", dan "Delete" pada tabel Chart of Account

- Update 1.7 (20 November 2023)

  - Pembuatan user interface untuk persiapan koneksi ke database.

- Update 1.8 (21 November 2023)

  - Pembuatan test database connection yang sudah bekerja.

- Update 1.9 (27 November 2023)

  - Menggunakan **Singkong** Versi 8.6.
  - Membuat repeat yang akan bekerja ketika konfigurasi database belum ada, karena aplikasi tidak dapat digunakan apabila belum konfigurasi ke database.
  - Aplikasi akan keluar dari repeat apabila sudah ditutup dengan tombol "Save" ataupun konfigurasi sudah tersedia.
  - Tidak add grid ke frame di setup.
  - Bug fix tidak bisa masuk ketika sudah keluar aplikasi.

- Update 2.0 (03 Desember 2023)

  - Penambahan credit pada aplikasi Bakwan.
  - Tombol "close" pada pengaturan database diubah menjadi "Quit" dan akan langsung menutup aplikasi tanpa meminta konfirmasi tambahan.
  - Komfirmasi penutupan frame sekarang hanya ditampilkan jika koneksi ke database berhasil, dengan menggunakan parameter konfigurasi dari file konfigurasi.
  - Jika terjadi kegagalan koneksi ke database, pengguna diberikan opsi untuk mereset konfigurasi. Contohnya jika parameter koneksi database tidak valid lagi, pengguna dapat memilih untuk tidak melakukannya, misalk=nya ketika database sedang offline.
  - Penambahan status bar yang menampilkan informasi mengenai status database, tanggal, dan waktu.

- Update 2.1 (05 Desember 2023)

  - Database telah disiapkan (pembuatan tabel dan pemasukan data) untuk keperluan otentikasi
  - Proses otentikasi telah berhasil untuk dilakukan.

- Update 2.2 (11 Desember 2023)

  - Menggunakan **Singkong** versi 8.7.
  - Pembaruan otomatis pada database, contohnya menambahkan aturan keterkaitan antar tabel (foreign key).
  - Penambahan menu bar.

- Update 2.3 (14 Desember 2023)

  - Perbaruan beberapa versi database aplikasi Bakwan.

- Update 2.4 (18 Desember 2023)

  - Perubahan nama table account pada database bakwan, karena account merupakan reserved atau key word pada salah satu sistem database.

- Update 2.5 (20 Desember 2023)

  - Database Bakwan sudah bisa menjalankan perintah "Create", "Update", dan "Delete" Chart of Account.

## Panduan Penggunaan Aplikasi

1. Pengguna dapat mengecek apakah bahasa pemrograman [**Java**](https://www.java.com/download/ie_manual.jsp) sudah terinstal di komputer pengguna, dikarenakan bahasa Singkong adalah sebuah interpreter yang kompatibel dengan bahasa pemrograman Java.

2. Pengguna dapat mengunduh bahasa pemrograman [**Singkong**](https://nopri.github.io/Singkong.jar) versi terbaru dan aplikasi [**Bakwan**](https://github.com/nopri/bakwan) di tautan yang tersedia.

3. Buka **Singkong.jar** yang telah diundur dari https://nopri.github.io/Singkong.jar.

4. Buka file **main.singkong** yang sudah diunduh dari https://github.com/nopri/bakwan. Lalu jalankan file tersebut.

5. Pengguna akan diberikan pesan bahwa database sudah berhasil diinisialisasi dan diberikan **username** serta **password default**. Pengguna juga akan diberikkan pesan bahwa database berhasil diperbarui sebelum kemudian diminta untuk memasukkan username dan password.

6. Pengguna memasukkan **username** dan **password** default yang telah diberikan sebelumnya.

7. Pengguna akan disajikan dua menu yaitu "**File**" dan "**Help**" :

   - Apabila pengguna memilih "**File**", maka user akan ditampilkan pilihan lain yaitu "**Setting**" dan "**Quit**".

     - Ketika pengguna memilih "**Setting**", maka pengguna akan disajikan tampilan "**Account Setup**" yang dimana pengguna dapat mengisi nama perusahaan, menentukan tahun fiskal, dan melakukan perubahan(menambahkan, menyunting, atau merubah) pada akun-akun.

     - Ketika pengguna memilih "**Quit**" maka pengguna akan dikeluarkan dari aplikasi Bakwan.

   - Apabila pengguna memilih "**Help**" maka pengguna akan ditampilkan pilihan "**About**".

8. Dalam tabel Chart Of Account akan terdapat ID, Type, Code, dan Description. Dalam tabel tersebut pengguna dapat:

   - menambahkan akun dengan tombol "**New**" dimana akan diminta mengisi Account Type, Code, dan Description.
   - Untuk menyunting akun, pengguna harus memilih baris yang diinginkan dan memilih tombol "**Edit**" yang akan mengubah bagian yang diinginkan dari ketiga hal tersebut.
   - Untuk menghapus salah satu akun, pengguna perlu memilih baris yang diinginkan sebelum menggunakan "**Delete**" lalu pengguna akan diminta konfirmasi kembali sebelum menghapus.

9. Jika sudah selesai, pengguna bisa menekan tombol "**Save**".

10. Jika sudah selesai menggunakan aplikasi, pengguna bisa menekan tombol "**Quit**" di menu "**File**"

## Referensi

- Epstein, L. (2007). _Bookkeeping Workbook_ For Dummies. Wiley.
