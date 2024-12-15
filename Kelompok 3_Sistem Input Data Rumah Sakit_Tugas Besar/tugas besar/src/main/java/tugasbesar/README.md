
# Panduan Penggunaan Aplikasi

Panduan ini memberikan instruksi langkah demi langkah untuk menggunakan aplikasi, termasuk login, navigasi menu, dan manajemen barang.

---

## Prasyarat

1. Pastikan Anda telah menginstal dan mengonfigurasi **JavaFX** di lingkungan pengembangan Anda.
2. Pastikan semua gambar yang digunakan dalam aplikasi berada di jalur file yang sesuai.
3. Kompilasi dan jalankan aplikasi menggunakan Java 8 atau versi yang lebih baru.

---

## Gambaran Fitur

## Fitur Utama

### 1. Login
- **Login Pasien**: Halaman login untuk pasien dengan kredensial statis.
- **Login Admin**: Halaman login untuk admin dengan kredensial statis.

### 2. Fitur untuk Admin
- **Menu Admin**: Halaman utama setelah login admin. Terdapat beberapa pilihan fitur:
    - **Daftar Pasien**: Menampilkan daftar pasien yang tersimpan.
    - **Daftar Obat**: Menampilkan daftar obat yang tersedia.
    - **Tambahkan Pasien**: Menambah data pasien baru ke sistem.
    - **Tambahkan Obat**: Menambah data obat baru ke sistem.
    - **Keluar**: Kembali ke halaman login.

### 3. Fitur untuk Pasien
- **Pengambilan Obat**: Memungkinkan pasien mengambil obat berdasarkan nomor antrian yang valid.
- **Pengembalian Obat**: Memungkinkan pasien mengembalikan obat dengan nomor antrian yang telah didaftarkan.




1. **Sistem Login**
    - Login Pengguna
    - Login Admin
2. **Navigasi Menu**
    - Menu Pengguna (Pembelian Barang)
    - Menu Admin
3. **Manajemen Barang**
    - Pembelian Barang
    - Pengembalian Barang

---

## Menjalankan Aplikasi

### Langkah 1: Jalankan Aplikasi

Jalankan file utama untuk menjalankan aplikasi:

```bash
java -cp . tugasbesar.LoginPasien
```

Layar login akan muncul.

---

### Langkah 2: Login sebagai Pengguna

1. Masukkan email dan kata sandi Anda di formulir login.
    - Contoh kredensial:
        - Email: `rumahsakit@gmail.com`
        - Kata Sandi: `12345`
2. Klik tombol **Login** untuk melanjutkan.
3. Jika kredensial benar, **Menu Pengguna** akan muncul.

#### Alternatif: Login sebagai Admin

1. Klik **Login Admin** untuk beralih ke formulir login admin.
2. Masukkan kredensial admin Anda:
    - Email: `rumahsakit@gmail.com`
    - Kata Sandi: `12345`
3. Klik **Login** untuk melanjutkan ke **Menu Admin**.

---

### Langkah 3: Navigasi Menu Pengguna

#### Pembelian obat

1. Di **Menu Pengguna**, klik **Beli obat**.
2. Telusuri obat yang tersedia di tabel.
3. Masukkan nomor barang di bidang input.
4. Klik **OK** untuk mengonfirmasi pembelian.
5. Jika barang tersedia, jumlahnya akan berkurang.

#### Pengembalian obat

1. Di **Menu Pengguna**, pilih **Pengembalian obat**.
2. Lihat obat yang di beli  di tabel.
3. Masukkan nomor obat untuk dikembalikan.
4. Klik **OK** untuk mengonfirmasi pengembalian.

---

### Langkah 4: Logout

1. Dari menu mana saja, klik **Keluar** untuk keluar dan kembali ke layar login.

---

## Catatan

1. Pastikan semua jalur file gambar dan koneksi database dikonfigurasi dengan benar.
2. Pesan kesalahan akan muncul jika input yang diberikan tidak benar.
    - Contoh: Kolom email atau kata sandi kosong.

Untuk detail lebih lanjut tentang kustomisasi kode atau pemecahan masalah, lihat file sumber atau hubungi tim pengembang.
 













## *TAMBAHAN*
## Cara Penggunaan
1. **Login Pasien**:
    - Jalankan `LoginPasien.java` untuk masuk sebagai pasien.
    - Masukkan kredensial:
        - Username: `rumahsakit@gmail.com`
        - Password: `12345`
    - Akses fitur pengambilan dan pengembalian obat.

2. **Login Admin**:
    - Jalankan `LoginAdmin.java` untuk masuk sebagai admin.
    - Masukkan kredensial:
        - Username: `rumahsakit@gmail.com`
        - Password: `12345`
    - Gunakan menu untuk mengelola pasien dan obat.

## Penjelasan Kode
- **LoginPasien.java** dan **LoginAdmin.java**: Mengelola proses login untuk masing-masing peran.
- **MenuAdmin.java**: Mengarahkan admin ke fitur manajemen pasien dan obat.
- **PasienAdd.java**: Menambahkan data pasien baru.
- **ObatAdd.java**: Menambahkan data obat baru.
- **ListPasien.java** dan **ListObat.java**: Menampilkan daftar pasien dan obat.
- **PengambilanObat.java** dan **Pengembalian.java**: Mengelola proses pengambilan dan pengembalian obat pasien.

## Catatan
- Data pasien dan obat hanya tersedia selama runtime aplikasi (tidak disimpan ke database).
- Pastikan semua file gambar berada pada jalur yang benar untuk menghindari error saat aplikasi dijalankan.

## Lisensi
Aplikasi ini bersifat open-source dan dapat dimodifikasi sesuai kebutuhan.