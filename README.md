# Pemrograman Mobile – Kumpulan Tugas

## Identitas Mahasiswa

| | |
|---|---|
| **Nama** | Adrian Akbar Firdaus |
| **NIM** | 41155050240017 |
| **Kelas** | Informatika A1 |
| **Mata Kuliah** | Pemrograman Mobile |

## Daftar Tugas

| Tugas | Topik | Folder |
|---|---|---|
| Tugas 2 | Aplikasi WebView Sederhana (MIT App Inventor) | [`Tugas2-AplikasiSederhana`](./Tugas2-AplikasiSederhana) |
| Tugas 3 | Implementasi WebView dengan Fabric React Native | [`Tugas3-WebView`](./Tugas3-WebView) |

---

## TUGAS 2 – Aplikasi Sederhana (WebView dengan MIT App Inventor)

### Deskripsi

Praktikum 2 membuat aplikasi mobile sederhana bernama **Kelompok 2** menggunakan MIT App Inventor. Aplikasi menampilkan halaman web eksternal (website Universitas Langlangbuana) langsung di dalam aplikasi Android menggunakan komponen WebView, dilengkapi tombol navigasi **Home** dan **Refresh**. Hasilnya berupa file proyek (`.aia`) dan file instalasi Android (`.apk`).

### Fitur Aplikasi

- Menampilkan halaman web eksternal di dalam aplikasi menggunakan komponen `WebView`.
- Tombol **Home** untuk kembali ke halaman awal.
- Tombol **Refresh** untuk memuat ulang halaman yang sedang dibuka.
- Label identitas kelompok (Adrian, Daniel, Miraj) di bagian atas layar.
- Dapat digunakan langsung di HP Android lewat file `.apk` tanpa membuka browser terpisah.

### Komponen yang Digunakan

| Komponen | Fungsi |
|---|---|
| `Screen1` | Layar utama aplikasi (judul "Kelompok 2"). |
| `HorizontalArrangement1` + `Label1` | Menampilkan nama anggota kelompok. |
| `HorizontalArrangement2` | Menata tombol Home dan Refresh secara horizontal. |
| `BtnHome` | Tombol untuk kembali ke halaman utama. |
| `BtnRefresh` | Tombol untuk memuat ulang halaman. |
| `WebView1` | Menampilkan halaman web eksternal. |

### Screenshot

**Tampilan desain di MIT App Inventor**

<img src="./screenshots/tugas2-app-inventor-desain.png" alt="Desain aplikasi di MIT App Inventor" width="600" />

**Tampilan aplikasi di HP Android**

<img src="./screenshots/tugas2-hasil-aplikasi.png" alt="Hasil aplikasi di HP Android" width="300" />

### Isi Folder

- `aplikasi_sederhana (1).aia` – file proyek App Inventor
- `aplikasi_sederhana.apk` – file instalasi aplikasi Android
- `Mobile-progamming-1` – materi/berkas pendukung
- `screenshots/` – gambar tampilan aplikasi

### Cara Menjalankan

1. Salin file `.apk` ke HP Android, lalu instal (izinkan instalasi dari sumber tidak dikenal).
2. Atau impor file `.aia` ke [MIT App Inventor](https://appinventor.mit.edu/) lewat menu **Projects → Import project (.aia)**.

---

## TUGAS 3 – Implementasi WebView dengan Fabric React Native

### Deskripsi

Praktikum 3 bertujuan mengimplementasikan tampilan web interaktif menggunakan komponen WebView pada React Native dengan mengaktifkan arsitektur baru (Fabric).

Aplikasi ini memungkinkan pengguna menampilkan dan mengakses halaman web eksternal langsung melalui aplikasi Android tanpa harus membuka browser secara terpisah.

### Fitur Aplikasi

- Menampilkan halaman web eksternal menggunakan komponen `react-native-webview`.
- Menggunakan arsitektur baru React Native (Fabric).
- Menggunakan komponen `SafeAreaView` dan `StatusBar`.
- Memiliki header kustom untuk tampilan antarmuka yang lebih menarik.
- Mendukung interaksi pengguna dengan halaman web di dalam aplikasi.

### Teknologi yang Digunakan

- React Native CLI
- React Native WebView
- Fabric (New Architecture)
- JavaScript
- Android Studio

### Instalasi dan Konfigurasi

**1. Clone Repository**

```bash
git clone https://github.com/adrian894399/pemogramanmobileAdrian
```

**2. Masuk ke Folder Proyek**

```bash
cd pemogramanmobileAdrian
```

**3. Instal Dependensi**

```bash
npm install
npm install react-native-webview
```

**4. Mengaktifkan Arsitektur Baru (Fabric)**

1. Buka folder `android` pada proyek.
2. Cari dan buka file `gradle.properties`.
3. Cari baris berikut:

   ```properties
   newArchEnabled=false
   ```

4. Ubah menjadi:

   ```properties
   newArchEnabled=true
   ```

5. Simpan perubahan dengan menekan `Ctrl + S`.

**5. Menyiapkan Perangkat Android**

*Menggunakan HP Android:*

1. Hubungkan HP ke laptop menggunakan kabel USB.
2. Aktifkan **Developer Options**.
3. Aktifkan **USB Debugging**.
4. Izinkan koneksi debugging jika muncul notifikasi pada HP.

*Menggunakan Emulator:*

1. Buka Android Studio.
2. Masuk ke **Device Manager**.
3. Jalankan emulator Android yang tersedia.
4. Tunggu hingga emulator siap digunakan.

### Cara Menjalankan Aplikasi

Setelah semua konfigurasi selesai, jalankan:

```bash
npx react-native run-android
```

Tunggu hingga proses build dan instalasi selesai. Aplikasi akan terbuka otomatis pada HP Android atau emulator.

### Komponen yang Digunakan

| Komponen | Fungsi |
|---|---|
| `WebView` | Menampilkan halaman web eksternal di dalam aplikasi. |
| `SafeAreaView` | Mengatur area aman tampilan aplikasi. |
| `StatusBar` | Mengatur tampilan status bar Android. |
| Header Custom | Menampilkan judul aplikasi. |

### Screenshot

<img width="328" height="623" alt="Screenshot 1" src="https://github.com/user-attachments/assets/62553769-ca3b-4640-bc53-8264536c6762" />
<img width="330" height="625" alt="Screenshot 2" src="https://github.com/user-attachments/assets/5f335998-3043-49d4-8cd7-af4e069156f6" />

---

## Kesimpulan

**Tugas 2:** Melalui praktikum ini, mahasiswa memahami pembuatan aplikasi mobile sederhana dengan MIT App Inventor, mulai dari merancang antarmuka dengan komponen visual, menggunakan WebView untuk menampilkan halaman web, hingga menambahkan tombol Home dan Refresh serta menghasilkan file APK.

**Tugas 3:** Penggunaan WebView pada React Native memungkinkan aplikasi mobile menampilkan halaman web eksternal secara langsung tanpa membuka browser terpisah. Library `react-native-webview` mempermudah integrasi halaman web ke dalam aplikasi, dan pengaktifan New Architecture (Fabric) memberikan dukungan sistem rendering React Native yang lebih modern. Mahasiswa memahami instalasi dependensi, konfigurasi Fabric, implementasi WebView, serta proses menjalankan aplikasi pada perangkat Android maupun emulator.

## Repository

- Repository utama: https://github.com/adrian894399/pemogramanmobileAdrian
- Sumber awal Tugas 2: https://github.com/adrian894399/-MobileProgramming_Session2
- Sumber awal Tugas 3: https://github.com/adrian894399/-MobileProgramming_Session3
