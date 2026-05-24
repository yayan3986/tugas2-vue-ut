## Tugas 2 Pemrograman Berbasis Web
Proyek membuat aplikasi Bahan Ajar UT dengan menggunakan framework Vue-js
Nama  : Septian Triputra
NIM   : 049841748

## Struktur Halaman

1. Halaman Stok Bahan Ajar
daftar stok bahan ajar yang terdiri dari kolom data field sebagai berikut :
o Kode Mata Kuliah/Nama Mata Kuliah → kode, judul
o Kategori Mata Kuliah → Kategori
o UT-Daerah → upbjj
o Lokasi Rak → lokasiRak
o Jumlah Stok Bahan Ajar → qty
o Jumlah Stok Safety Bahan Ajar → safety
o Status
o Catatan → catatanHTML

2. Tracking Delivery Order (DO)
Terdapat fitur untuk menambahkan input delivery order yang baru. Berikut adalah data
field yang perlu diisi
o Nomor DO, di mana tergenerate otomatis. Penomorannya terdiri dari:
▪ DO
▪ Tahun Berjalan
▪ Sequence Number
Misal:
DO2025-001 untuk data awal
Selanjutnya jika sudah ada data tracking terbaru, menjadi DO2025-002 dst.
o NIM, diisi secara manual oleh pengguna
o Nama, diisi secara manual oleh pengguna
o Ekspedisi (JNE Regular/JNE Express), dipilih oleh pengguna berdasarkan data
pada upbjjList
o Paket Bahan Ajar, dipilih oleh pengguna berdasarkan data pada paket
▪ Gunakan elemen <select> dan menampilkan di halaman web informasi
kode paket dan nama paket
▪ Setelah memilih paket, akan muncul detail isi paket bahan ajar tersebut
di bawah elemen <select> untuk memberikan informasi
o Tanggal Kirim, dapat diisi manual ataupun menggunakan fungsi Date untuk
mengambil local time.
o Total Harga, diambil dari data pada Array of Objects paket → harga

### Untuk menjalankan proyek di terminal dengan perintah berikut

```sh
npm run dev
```
