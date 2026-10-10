# Sidance 2.5 Motion Control Web App

Web app statis ramah HP untuk memilih video referensi dan foto karakter, melihat pratinjau, mengatur durasi/rasio, lalu membuat prompt motion-control yang bisa disalin atau diunduh.

## Jalankan di HP/komputer
Buka `index.html` di browser modern. Tidak membutuhkan instalasi atau API untuk fungsi pratinjau dan pembuatan prompt.

## Deploy gratis dengan GitHub Pages
1. Buat repositori GitHub baru, misalnya `sidance-2-5`.
2. Unggah `index.html` dan `README.md` ke root repositori.
3. Buka **Settings → Pages**.
4. Di **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/(root)`, lalu tekan **Save**.
6. Tunggu proses selesai dan buka URL GitHub Pages yang ditampilkan di bagian Pages.

## Batasan penting
Versi ini belum menghasilkan video jadi. Tombol Generate Video memvalidasi bahwa kedua input tersedia dan menyusun prompt. Untuk motion transfer/render sungguhan, perlu menghubungkan model/layanan video AI yang mendukung video referensi + gambar karakter. Jangan menaruh API key rahasia di JavaScript frontend; gunakan backend/serverless function jika nanti menghubungkan API.
