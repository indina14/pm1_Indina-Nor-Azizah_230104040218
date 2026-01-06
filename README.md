# pm1_Indina-Nor-Azizah_230104040218

Laporan Praktikum 1: Mobile Programming
Aplikasi Android sederhana berbasis Kotlin yang mendemonstrasikan konsep dasar interaksi User Interface (UI) dan Event Handling pada Android Studio.
# Deskripsi Tugas
Tujuan dari praktikum ini adalah membuat aplikasi "Hello World" yang interaktif. Aplikasi dapat mengubah isi teks (TextView) secara dinamis ketika pengguna menekan sebuah tombol (Button) dengan menerapkan logika toggle menggunakan variabel status.
# Persiapan (Tech Stack)
Bahasa Pemrograman: Kotlin
IDE: Android Studio
Library: AndroidX AppCompat
Perangkat Uji: Vivo V2205 (API Level 34)
#Struktur Proyek
File,Deskripsi
MainActivity.kt,Logika pemrograman untuk menangani klik tombol.
activity_main.xml,Definisi tata letak (layout) UI aplikasi.
AndroidManifest.xml,Konfigurasi dasar aplikasi Android.
#Implementasi Kode
Logika Utama (MainActivity.kt)
Kode ini menggunakan findViewById untuk menghubungkan komponen UI dan setOnClickListener untuk logika interaksi:
// Inisialisasi status awal
var isHalo = true

btnToggle.setOnClickListener {
    if (isHalo) {
        tvMessage.text = "Selamat Datang di Perkuliahan Mobile Programming"
        isHalo = false
    } else {
        tvMessage.text = "Halo Indina"
        isHalo = true
    }
}

#Hasil Running
Aplikasi memiliki dua kondisi utama (State) yang berubah secara bergantian setiap kali tombol "Klik Saya" ditekan:
1. State Awal / Kondisi A
Menampilkan pesan selamat datang di perkuliahan.
Pesan: "Selamat Datang di Perkuliahan Mobile Programming"
2. State Kedua / Kondisi B
Menampilkan sapaan personal.
Pesan: "Halo Indina"

📝 Kesimpulan
Pada praktikum ini, beberapa poin penting yang dipelajari adalah:
Cara menghubungkan elemen XML ke dalam file Kotlin menggunakan ID.
Penggunaan variabel Boolean sebagai penanda status (flagging).
Penerapan struktur kontrol If-Else untuk menciptakan antarmuka yang dinamis.
