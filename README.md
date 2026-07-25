# Log Garasi 🏋️ — Pelacak Latihan Rumahan

Aplikasi web sederhana (satu file `index.html`, tanpa perlu install apa pun) untuk melacak latihan harian pakai handgrip, galon Le Minerale, dumbbell 6kg, alat bantu sit-up, dan pull-up bar.

## Fitur
- Jadwal mingguan otomatis (Senin–Minggu) sesuai fokus otot per hari
- Centang ✅ tiap latihan yang sudah selesai
- Hitungan repetisi per kelipatan **5 reps** (tombol +/−), divisualisasikan seperti tumpukan plat beban
- Unggah foto/gambar contoh gerakan untuk tiap latihan (tersimpan di browser)
- Tanggal otomatis mengikuti kalender asli, bisa juga pilih tanggal lain
- Riwayat harian tersimpan otomatis
- Tombol **Ekspor CSV** untuk mengunduh seluruh riwayat

## Cara pakai di GitHub Pages (gratis, tanpa server)
1. Buat repository baru di GitHub, misalnya `log-garasi`.
2. Upload file `index.html` ini ke repository tersebut (lewat "Add file → Upload files").
3. Buka **Settings → Pages** di repository.
4. Pada bagian **Source**, pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
5. Tunggu 1-2 menit, GitHub akan memberi link seperti:
   `https://<username-kamu>.github.io/log-garasi/`
6. Buka link itu di HP atau laptop — aplikasi siap dipakai.

## Catatan penting soal penyimpanan data
Data (centang, jumlah reps, foto, riwayat) disimpan di **localStorage browser** kamu masing-masing perangkat/browser. Artinya:
- Data **tidak otomatis sinkron** antara HP dan laptop, atau antar browser berbeda.
- Kalau kamu membersihkan cache/data browser, riwayat bisa hilang.
- Karena itu, gunakan tombol **Ekspor CSV** secara berkala untuk cadangan data kamu.

## Struktur latihan
| Hari | Fokus |
|---|---|
| Senin | Lengan & Bahu |
| Selasa | Kaki |
| Rabu | Istirahat |
| Kamis | Punggung & Tarikan |
| Jumat | Core + Kaki Ringan |
| Sabtu | Full Body Kombinasi |
| Minggu | Istirahat Total |

Semua target reps sudah disusun dalam kelipatan 5 agar mudah dihitung dengan tombol +5/-5 di aplikasi.

## Mengubah latihan
Buka `index.html` dengan text editor apa pun, cari bagian `const EXERCISES = [...]` di dalam tag `<script>`, lalu edit nama, jumlah set/reps, hari, atau alat sesuai kebutuhanmu.
