# Portofolio BTC: panduan pasang di Android

Isi paket:
- index.html  (aplikasinya)
- manifest.json, sw.js, icons/  (agar bisa dipasang dan jalan offline)

Data pembelian disimpan di perangkat yang dipakai (localStorage). Gunakan tombol
"Unduh cadangan (JSON)" di aplikasi secara berkala dan simpan file-nya di Google Drive.
Harga BTC diisi manual.

## Cara 1: pasang sebagai aplikasi (PWA), tanpa APK

1. Buat akun GitHub (gratis), lalu buat repository baru, misalnya `portofolio-btc`, set Public.
2. Klik "Add file" > "Upload files", unggah SEMUA isi folder ini (index.html, manifest.json,
   sw.js, dan folder icons). Klik "Commit changes".
3. Buka Settings > Pages. Pada "Branch" pilih `main` dan folder `/ (root)`, klik Save.
4. Tunggu 1-2 menit. Alamatnya: https://NAMA-GITHUB-ANDA.github.io/portofolio-btc/
5. Buka alamat itu di Chrome Android. Ketuk menu titik tiga > "Instal aplikasi"
   (atau "Tambahkan ke layar utama"). Ikon Portofolio BTC muncul di layar utama.

Alternatif hosting: Netlify Drop (app.netlify.com/drop), seret folder ini ke halamannya.

## Cara 2: file APK

Kerjakan Cara 1 sampai alamatnya bisa dibuka. Lalu:

1. Buka https://www.pwabuilder.com dan masukkan alamat dari langkah 4.
2. Klik Start, tunggu analisis, lalu "Package for stores" > Android.
3. Isi nama paket (contoh: com.namaanda.portofoliobtc), lalu Generate.
4. Unduh file ZIP. Di dalamnya ada file .apk (untuk dipasang langsung) dan .aab (untuk Play Store).
5. Salin .apk ke HP, buka, dan izinkan "Pasang dari sumber tidak dikenal" jika diminta.

Catatan: APK dari PWABuilder membuka alamat web Anda di dalam aplikasi. Jika Anda mengubah
index.html dan mengunggah ulang, naikkan angka versi di sw.js (portofolio-btc-v1 jadi v2)
supaya HP memuat versi terbaru.

## Cara mengubah
Edit index.html. Seluruh tampilan dan perhitungan ada di satu file itu.
