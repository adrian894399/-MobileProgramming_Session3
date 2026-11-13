## TUGAS 3 – IMPLEMENTASI WEBVIEW DENGAN FABRIC REACT NATIVE
Identitas Mahasiswa
Nama: Adrian Akbar Firdaus
NIM: 41155050240017
Kelas: Informatika A1
Mata Kuliah: Pemrograman Mobile
Deskripsi

## Praktikum 3 ini bertujuan untuk mengimplementasikan tampilan web interaktif menggunakan komponen WebView pada React Native dengan mengaktifkan arsitektur baru (Fabric).

Aplikasi ini memungkinkan pengguna menampilkan dan mengakses halaman web eksternal secara langsung melalui aplikasi Android tanpa harus membuka browser secara terpisah.

## Fitur Aplikasi
Menampilkan halaman web eksternal menggunakan komponen react-native-webview.
Menggunakan arsitektur baru React Native (Fabric).
Menggunakan komponen SafeAreaView dan StatusBar.
Memiliki Header kustom untuk tampilan antarmuka yang lebih menarik.
Mendukung interaksi pengguna dengan halaman web di dalam aplikasi.
Teknologi yang Digunakan
React Native CLI
React Native WebView
Fabric (New Architecture)
JavaScript
Android Studio
## Instalasi dan Konfigurasi
1. Clone Repository
bash
git clone https://github.com/adrian894399/pemogramanmobileAdrian

2. Masuk ke Folder Proyek
bash
cd pemogramanmobileAdrian

3. Instal Dependensi

Jalankan perintah berikut di terminal:

bash
npm install
npm install react-native-webview

4. Mengaktifkan Arsitektur Baru (Fabric)
Buka folder android pada proyek.
Cari dan buka file gradle.properties.
Cari baris berikut:
properties
newArchEnabled=false

Ubah menjadi:
properties
newArchEnabled=true

Simpan perubahan dengan menekan Ctrl + S.
5. Menyiapkan Perangkat Android

## Menggunakan HP Android:

Hubungkan HP ke laptop menggunakan kabel USB.
Aktifkan Developer Options.
Aktifkan USB Debugging.
Izinkan koneksi debugging jika muncul notifikasi pada HP.

## Menggunakan Emulator:

Buka Android Studio.
Masuk ke Device Manager.
Jalankan emulator Android yang tersedia.
Tunggu hingga emulator siap digunakan.
Cara Menjalankan Aplikasi

## Setelah semua konfigurasi selesai, jalankan perintah berikut:

bash
npx react-native run-android


Tunggu hingga proses build dan instalasi selesai. Aplikasi akan terbuka secara otomatis pada HP Android atau emulator.

Komponen yang Digunakan
Komponen	Fungsi
WebView	Menampilkan halaman web eksternal di dalam aplikasi.
SafeAreaView	Mengatur area aman tampilan aplikasi.
StatusBar	Mengatur tampilan status bar Android.
Header Custom	Menampilkan judul aplikasi.
Kesimpulan

Berdasarkan Praktikum 2 yang telah dilakukan, dapat disimpulkan bahwa penggunaan WebView pada React Native memungkinkan aplikasi mobile untuk menampilkan halaman web eksternal secara langsung tanpa harus membuka browser terpisah.

Penggunaan library react-native-webview mempermudah integrasi halaman web ke dalam aplikasi. Selain itu, pengaktifan New Architecture (Fabric) memberikan dukungan terhadap sistem rendering React Native yang lebih modern.

Melalui praktikum ini, mahasiswa dapat memahami instalasi dependensi, konfigurasi Fabric, implementasi WebView, serta proses menjalankan aplikasi React Native pada perangkat Android maupun emulator.

Repository GitHub:
https://github.com/adrian894399/pemogramanmobileAdrian

## SreenShoot
<img width="328" height="623" alt="image" src="https://github.com/user-attachments/assets/62553769-ca3b-4640-bc53-8264536c6762" />
<img width="330" height="625" alt="image" src="https://github.com/user-attachments/assets/5f335998-3043-49d4-8cd7-af4e069156f6" />
