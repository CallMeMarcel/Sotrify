# Sotrify: Spotify Clone App

Aplikasi pemutar musik *multi-platform* yang dibangun menggunakan **Flutter**, meniru fungsionalitas Spotify dengan fokus pada desain UI/UX yang bersih dan modern. Proyek ini mengimplementasikan **Clean Architecture** dan **BLoC State Management** untuk skalabilitas dan pemeliharaan kode yang terstruktur.

---

## 🌟 Fitur Utama

Berdasarkan dependensi dan struktur file proyek:

* **Autentikasi Pengguna:**
    * Mendukung proses pendaftaran (*Sign Up*) dan masuk (*Sign In*).
    * Menggunakan **Firebase Authentication** untuk manajemen akun pengguna.
    * Pengambilan data profil pengguna setelah autentikasi.
* **Pemutar Audio:**
    * Fungsionalitas pemutaran lagu dasar menggunakan paket `just_audio`.
    * Dilengkapi dengan tampilan Pemutar Lagu (*Song Player*) dengan kontrol status putar.
* **Katalog Musik:**
    * Menampilkan daftar lagu baru (*News Songs*).
    * Menampilkan daftar putar (*Playlist*) yang dapat dijelajahi.
* **Manajemen Favorit:**
    * Fitur untuk menambah atau menghapus lagu dari daftar favorit pengguna.
    * Mengecek status apakah sebuah lagu sudah menjadi favorit.
    * Melihat daftar lagu favorit di halaman profil.
* **Pilihan Tema:**
    * Dukungan untuk beralih antara tema terang dan gelap (*Light/Dark Mode*).

---

## 💻 Teknologi yang Digunakan

Proyek ini dibangun menggunakan **Flutter** dan memanfaatkan beberapa paket kunci untuk implementasi arsitektur dan fungsionalitas *backend*.

| Kategori | Teknologi/Paket | Versi (dari `pubspec.yaml`) |
| :--- | :--- | :--- |
| **Framework** | **Flutter** | `sdk: '>=3.1.3 <4.0.0'` |
| **State Management** | `flutter_bloc` | `^8.1.6` |
| **State Persistence** | `hydrated_bloc` | `^9.1.5` |
| **Backend/Auth** | `firebase_auth` | `^5.3.2` |
| **Database** | `cloud_firestore` | `^5.4.5` |
| **Audio Playback** | `just_audio` | `^0.9.42` |
| **Dependency Injection** | `get_it` | `^8.0.2` |
| **Fungsional (Monads)** | `dartz` | `^0.10.1` |
| **Utility** | `path_provider` | `^2.1.5` |
| **UI/Aset** | `flutter_svg` | `^2.0.14` |

---

## 🛠 Prasyarat Instalasi

1.  **Flutter SDK**
    * Instal dan konfigurasikan Flutter SDK (versi yang disarankan `>=3.1.3`).
2.  **Proyek Firebase**
    * Buat proyek baru di [Firebase Console](https://console.firebase.google.com/).
    * Aktifkan **Firebase Authentication** dan **Cloud Firestore**.
    * Tambahkan aplikasi Android dan/atau iOS ke proyek Firebase Anda.
3.  **Konfigurasi Firebase**
    * Unduh file konfigurasi Firebase yang sesuai:
        * Untuk Android: Letakkan `google-services.json` di direktori `android/app/`.
        * Untuk iOS: Konfigurasikan proyek Anda.
    * File `firebase_options.dart` juga akan dibuat setelah konfigurasi CLI.

---

## 📂 Susunan Project

Proyek ini mengadopsi prinsip **Clean Architecture** (berdasarkan struktur file dalam direktori `lib`)

## ▶️ Contoh Penggunaan

Setelah menginstal semua prasyarat dan mengkloning repositori:

1.  **Ambil Dependensi:**
    ```bash
    flutter pub get
    ```

2.  **Inisialisasi Service Locator:**
    Pastikan `service_locator.dart` telah dipanggil di `main.dart` sebelum menjalankan aplikasi.

3.  **Jalankan Aplikasi:**
    ```bash
    flutter run
    ```

Aplikasi akan dimulai dengan:
* **Splash Screen**
* **Halaman Perkenalan (*Get Started*)**
* **Pilihan Mode Tema** (*Light/Dark Mode*)
* **Halaman Autentikasi** (*Sign Up/Sign In*)

Setelah masuk, Anda akan diarahkan ke **Halaman Utama (*Home*)** untuk melihat daftar lagu dan playlist.

---

## 🤝 Kontribusi

Kami sangat menghargai kontribusi dari komunitas! Untuk berkontribusi:

1.  *Fork* repositori ini.
2.  Buat *branch* baru untuk fitur Anda (`git checkout -b fitur/nama-fitur`).
3.  Pastikan kode Anda mengikuti linter project (`flutter_lints: ^2.0.0`).
4.  Lakukan *commit* dan *push* perubahan Anda.
5.  Ajukan *Pull Request* (PR) ke *branch* utama.

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **Lisensi MIT**.
