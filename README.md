# 📱 Data Siswa App

Aplikasi Android untuk mengelola data siswa yang dikembangkan menggunakan **Kotlin** dan **Jetpack Compose**. Aplikasi ini memungkinkan pengguna melihat daftar siswa dan menambahkan data siswa melalui koneksi REST API.

## ✨ Fitur Aplikasi

- Menampilkan daftar data siswa.
- Menambahkan data siswa baru.
- Menginput nama, alamat, dan nomor telepon siswa.
- Validasi input sebelum menyimpan data.
- Mengambil dan mengirim data melalui REST API.
- Navigasi antarhalaman menggunakan Navigation Compose.

## 🛠️ Teknologi yang Digunakan

- Kotlin
- Jetpack Compose
- Material Design 3
- MVVM Architecture
- Retrofit
- Kotlinx Serialization
- Navigation Compose
- REST API

## 📸 Tampilan Aplikasi

### 1. Halaman Home
Menampilkan daftar data siswa yang berhasil diambil dari server.

<img width="382" height="857" alt="Screenshot 2026-11-26 232802" src="https://github.com/user-attachments/assets/f5acd1a6-38ad-4abb-98de-a2fdbc5f44e3" />

### 2. Halaman Tambah Siswa
Halaman untuk memasukkan data siswa berupa nama, alamat, dan nomor telepon.

<img width="378" height="853" alt="Screenshot 2026-11-26 232901" src="https://github.com/user-attachments/assets/a70f7d46-652c-4022-b30d-9cdbe50b4608" />

### 3. Form Input Siswa
Tampilan form pengisian data siswa sebelum disimpan.

<img width="385" height="855" alt="Screenshot 2026-11-26 232912" src="https://github.com/user-attachments/assets/3611904e-5dc3-4ee1-b606-573dbbfe2a83" />

## 📂 Struktur Project

```text
com.example.mydatasiswa
│
├── apiservice
│   └── ServiceApiSiswa.kt
│
├── modeldata
│   └── DataSiswa.kt
│
├── repositori
│   ├── RepositoryDataSiswa.kt
│   ├── ContainerApp.kt
│   └── AplikasiDataSiswa.kt
│
├── view
│   ├── DestinasiNavigasi.kt
│   ├── DestinasiHome.kt
│   ├── DestinasiEntry.kt
│   ├── HomeScreen.kt
│   ├── EntrySiswaScreen.kt
│   └── SiswaTopAppBar.kt
│
└── viewmodel
    ├── HomeViewModel.kt
    ├── EntryViewModel.kt
    └── PenyediaViewModel.kt
```

## ⚙️ Konfigurasi

Sebelum menjalankan aplikasi, pastikan server REST API sudah aktif dan sesuaikan alamat server pada konfigurasi Retrofit:

```kotlin
private val baseurl = "http://10.0.2.2/umyTI/"
```

Pastikan endpoint API berikut tersedia:

- `bacaTeman.php` — mengambil data siswa.
- `insertTM.php` — menambahkan data siswa.

## 🚀 Cara Menjalankan

1. Clone repository ini.
2. Buka project menggunakan Android Studio.
3. Pastikan konfigurasi server API sudah sesuai.
4. Jalankan server backend.
5. Sync Gradle.
6. Jalankan aplikasi menggunakan emulator atau perangkat Android.

---

**Developed with ❤️ using Kotlin and Jetpack Compose.**
