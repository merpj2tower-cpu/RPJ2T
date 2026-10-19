CATATAN METER AIR RUSUN PULO JAHE TOWER — proyek Android

PENTING: Ini adalah kode sumber Android, bukan file APK siap instal. Workflow GitHub Actions sudah disiapkan untuk membuat APK secara otomatis.

CARA MEMBUAT APK DI GITHUB:
1. Login ke GitHub dan buat repository baru (misalnya: CatatanMeterAir).
2. Ekstrak ZIP ini di HP/komputer.
3. Upload SELURUH ISI folder hasil ekstrak ke ROOT repository. Pastikan folder .github/workflows/build-apk.yml terlihat di root repository (bukan berada di dalam folder proyek lain).
4. Buka tab Actions. Jika diminta, izinkan Actions untuk repository.
5. Pilih workflow "Build APK", tekan Run workflow, lalu Run workflow lagi untuk konfirmasi.
6. Tunggu sampai proses selesai dengan tanda hijau/success.
7. Buka proses workflow yang berhasil, scroll ke bagian Artifacts, lalu download "CatatanMeterAir-debug-apk".
8. Ekstrak ZIP artifact dan instal app-debug.apk di HP Android. Jika diminta, izinkan instalasi dari sumber ini.

Build juga berjalan otomatis saat perubahan di-push ke branch main atau master.

STATUS FITUR:
- Halaman aplikasi dimuat dari file HTML lokal.
- Catatan disimpan di localStorage dalam WebView aplikasi.
- Input kamera/pemilih foto tersedia.
- OCR Tesseract.js dan ekspor ExcelJS pada halaman saat ini menggunakan CDN internet, jadi kedua fitur tersebut memerlukan internet dan belum sepenuhnya offline.
- APK yang dibuat adalah debug APK untuk uji coba. Data lokal bisa hilang jika data aplikasi dihapus atau aplikasi di-uninstall; lakukan backup berkala.

Jika build gagal, buka run di tab Actions dan kirimkan log error merahnya agar bisa diperbaiki.
