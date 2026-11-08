# Aplikasi Daftar Produk Toko (JavaFX)

Aplikasi desktop berbasis JavaFX dan Maven untuk pencatatan, pencarian, serta melihat detail daftar produk toko (kategori **Makanan** dan **Minuman**).

## Fitur Utama
- **Form Tambah Produk (`form.fxml`):** Menambahkan produk baru dengan validasi nama produk tidak boleh kosong dan harga harus lebih dari nol.
- **Daftar Produk (`daftar.fxml`):** Menampilkan tabel berisi kode produk, nama produk, kategori, dan harga.
- **Pencarian Produk:** Mencari produk berdasarkan nama melalui tombol **Cari** (atau menekan tombol **Enter**).
- **Detail Produk (`detail.fxml`):** Menampilkan rincian lengkap dari objek produk yang dipilih pada tabel atau setelah data baru disimpan.

## Struktur Proyek
- `src/main/java/kelas/MainApp.java` — Entry point aplikasi JavaFX.
- `src/main/java/kelas/Navigator.java` — Mengatur perpindahan halaman (`daftar`, `form`, `detail`) dalam satu `Stage`.
- `src/main/java/kelas/model/Produk.java` — Class model produk beserta validasi input.
- `src/main/java/kelas/data/DataProduk.java` — Penyimpanan daftar produk sementara di memori selama aplikasi berjalan.
- `src/main/java/kelas/controller/` — Controller untuk masing-masing tampilan (`DaftarController`, `FormController`, `DetailController`).
- `src/main/resources/kelas/` — File antarmuka FXML (`daftar.fxml`, `form.fxml`, `detail.fxml`) dan stylesheet (`styles/app.css`).

## Cara Menjalankan Aplikasi

### Opsi 1: Menggunakan Apache NetBeans
1. Pastikan **JDK 17+** dan **Apache NetBeans** sudah terinstal.
2. Download atau clone repository ini (**Code > Download ZIP**, lalu ekstrak).
3. Di NetBeans, pilih **File > Open Project**, lalu arahkan ke folder proyek.
4. Klik kanan pada proyek di panel **Projects**, pilih **Clean and Build**.
5. Klik **Run Project** (`F6`) untuk menjalankan `kelas.MainApp`.

### Opsi 2: Menggunakan Terminal (Maven)
1. Buka terminal dan masuk ke folder utama proyek (lokasi file `pom.xml`).
2. Jalankan perintah berikut:
   ```bash
   mvn clean javafx:run

## Screenshot
### Daftar Produk
<img width="906" height="714" alt="image" src="https://github.com/user-attachments/assets/dbf97c4f-04d0-411e-9213-e9d488177a81" />
### Pencarian Produk
<img width="898" height="709" alt="image" src="https://github.com/user-attachments/assets/a2cba9e5-0046-4c28-820f-0da5aa400ca5" />
### Detail PRoduk
<img width="902" height="708" alt="image" src="https://github.com/user-attachments/assets/f36b186b-8473-4be3-9544-5a9d94bd1f30" />
### Tambah Produk
<img width="898" height="704" alt="image" src="https://github.com/user-attachments/assets/6846a2e9-d24d-4913-aa87-4f079e7ccf3b" />

