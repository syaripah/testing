# Cara membuat APK PIXELSCAN Mobile

## Cara 1 - Online lewat GitHub (tanpa install Android Studio)
1. Buat repo GitHub baru, unggah isi folder ini (tanpa node_modules dan android).
2. Buka tab **Actions** > **Build APK** > **Run workflow**.
3. Tunggu sekitar 5-10 menit, lalu unduh **PIXELSCAN-debug-apk** dari bagian Artifacts.
4. Ekstrak zip-nya, kirim `app-debug.apk` ke HP, lalu pasang (izinkan "install dari sumber tidak dikenal").

## Cara 2 - Di laptop
Syarat: Node 20+, JDK 21, Android SDK (paling mudah lewat Android Studio).
```
npm install
npm run android:apk
```
Hasil: `android/app/build/outputs/apk/debug/app-debug.apk`

## Setelah terpasang
- Floating bubble butuh izin "Tampilkan di atas aplikasi lain".
- Auto-scroll butuh Aksesibilitas: Pengaturan > Aksesibilitas > PIXELSCAN Mobile > aktifkan.
