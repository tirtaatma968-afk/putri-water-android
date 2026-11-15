# Build APK lewat HP (GitHub Actions)

Paket ini sudah menyertakan workflow cloud build di `.github/workflows/build-apk.yml`.

1. Buat akun GitHub atau masuk di github.com.
2. Buat repository baru, misalnya `putri-water-app`.
3. Upload seluruh isi folder proyek ini ke repository (termasuk folder `.github`). Jangan upload folder pembungkus hasil ekstrak; upload isi di dalamnya.
4. Buka tab **Actions** pada repository. Jika diminta, aktifkan Actions.
5. Pilih workflow **Build PUTRI WATER APK**, tekan **Run workflow**.
6. Setelah selesai dengan status hijau, buka hasil run dan unduh artifact `putri-water-debug-apk`.
7. Ekstrak artifact ZIP di HP; di dalamnya ada `app-debug.apk`.

Catatan: ini hanya mengompilasi source menjadi APK debug. Aplikasi belum siap dipakai online sampai URL dan publishable key Supabase di `app/src/main/assets/config.js` diisi dan skema database dipasang dengan aman. Jangan pernah memasukkan service_role/secret key ke aplikasi Android.
