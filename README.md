# Bio Accoustic OS (BAO)

Aplikasi frekuensi biologis pintar dengan 11 mode frekuensi kesehatan, terintegrasi AdMob dinamis via Panel Admin lokal, dan sistem Auto-Update tanpa uninstall.

## 🚀 Cara Instal & Update via GitHub

1. Ekstrak file zip ini.
2. Upload semua file (kecuali folder `.github` jika menggunakan web GitHub, lihat poin 3) ke root repositori Anda.
3. Untuk file `main.yml`, Anda harus membuatnya di dalam folder repositori Anda dengan letak persis: `.github/workflows/main.yml`, lalu *copy-paste* isinya ke sana.
4. Buka tab **Actions** di GitHub, tunggu proses `Auto Build APK Android` selesai (warna hijau).
5. Scroll ke bawah, unduh **BAO-App-APK** di bagian *Artifacts*.
6. Ekstrak dan instal di HP Android Anda.

## 💰 Cara Set AdMob (Tanpa Koding)

1. Buka aplikasi **BAO** di HP Anda.
2. Ketuk logo **BAO** (Lingkaran Putih) di bagian atas layar sebanyak **5 kali secara cepat**.
3. *Panel Admin* akan muncul. Masukkan **AdMob App ID** & **Ad Unit ID Banner** Anda.
4. Restart aplikasi. Iklan akan muncul di bagian bawah jika ID benar (pastikan Anda sudah mengubah status `isTesting` dari `true` ke `false` di `index.html` jika siap rilis Play Store).

## 🔄 Cara Menjalankan Sistem Auto-Update

Ketika Anda ingin merilis perbaikan:
1. Naikkan angka `versionCode` dan `versionName` di dalam file `version.json`.
2. Ubah juga `APP_VERSION_CODE` di `index.html` agar selaras.
3. Pastikan `downloadUrl` di file `version.json` sudah diisi dengan link *direct download* ke APK baru Anda.
4. Saat pengguna membuka aplikasinya, akan muncul *pop-up* pembaruan!
