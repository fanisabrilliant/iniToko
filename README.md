# iniToko
Aplikasi desktop sederhana untuk mengelola daftar produk toko, dibuat dengan **JavaFX 21** dan **Maven**. Pengguna bisa menambah produk, mencari produk berdasarkan nama, dan melihat detail produk dalam tiga halaman yang saling terhubung.

## fitur
1. Tambah produk dengan nama, kategori (Makanan / Minuman), dan harga.
2. Kode produk otomatis  berformat `PR001`, `PR002`, dan seterusnya.
3. Validasi input: nama wajib diisi, harga harus angka bulat lebih dari nol, kategori hanya Makanan atau Minuman. Pesan error tampil merah, pesan sukses tampil hijau.
4. Daftar produk dalam tabel dengan harga berformat rupiah (contoh `Rp15.000`).
5. Pencarian nama produk, lengkap dengan tombol Reset dan jumlah data yang tampil.
6. Detail produk untuk baris yang dipilih di tabel.
7. Tampilan dengan CSS dan layout FXML

---

## Tampilan Aplikasi

### 1. Halaman Tambah Produk
Halaman pertama yang terbuka saat aplikasi dijalankan.

<img width="1112" height="882" alt="Screenshot 2026-11-09 225303" src="https://github.com/user-attachments/assets/78945ef4-cd88-4670-aaed-6fb5b8a4dce8" />


Setelah produk berhasil disimpan, form dikosongkan otomatis supaya bisa langsung input produk berikutnya:

<img width="1122" height="880" alt="image" src="https://github.com/user-attachments/assets/a9616194-bc14-4a1b-9618-4288d9711efd" />


Jika input salah, pesan error ditampilkan di bawah tombol:

<img width="1115" height="872" alt="Screenshot 2026-11-09 225344" src="https://github.com/user-attachments/assets/324409c3-a582-4397-bc3c-759915dc24b5" />


### 2. Halaman Daftar Produk
Tabel berisi semua produk. Ketik di kolom cari lalu tekan **Enter** atau tombol **Cari**. Pilih satu baris lalu klik **Lihat Detail**.

<img width="1117" height="851" alt="image" src="https://github.com/user-attachments/assets/587435ad-9b2e-4c62-be45-84b734aa591a" />


### 3. Halaman Detail Produk
Menampilkan kode, nama, kategori, dan harga produk yang dipilih.

<img width="1110" height="875" alt="image" src="https://github.com/user-attachments/assets/bf2ae188-3c20-462e-9b71-7248bd761c42" />


## Cara Menjalankan

### Prasyarat
- **JDK 17 atau lebih baru** (cek dengan `java -version`)
- **Maven** (cek dengan `mvn -version`)

### Lewat terminal

```bash
git clone https://github.com/<username>/IniToko.git
cd IniToko
mvn javafx:run
```

Maven akan mengunduh JavaFX otomatis saat pertama kali dijalankan, jadi butuh koneksi internet.

### Lewat NetBeans
1. Buka **File → Open Project**, pilih folder `IniToko`.
2. Klik kanan proyek → **Run** (atau tekan `F6`).


