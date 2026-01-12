# FIFO Master

Aplikasi web untuk cleaning data dan integrasi FIFO (First In, First Out) untuk logistik barang. Aplikasi ini memungkinkan pengguna untuk membersihkan data dari file Excel, kemudian melakukan perhitungan FIFO untuk stok barang masuk dan keluar.

## Fitur Utama

- **Data Cleaning**: Bersihkan dan format data dari file Excel (SO/Stok Awal, Barang Masuk, Barang Keluar).
- **Integrasi FIFO**: Hitung stok FIFO berdasarkan data barang masuk dan keluar, dengan dukungan kolom tambahan opsional.
- **Ekspor Hasil**: Unduh hasil cleaning dan FIFO dalam format Excel.

## Persyaratan Sistem

- Windows 10/11
- Tidak memerlukan instalasi Python atau dependensi lainnya (aplikasi sudah dibundel sebagai executable).

## Cara Menggunakan

1. **Unduh Aplikasi**: Unduh file `app.exe` dari folder `dist/`.
2. **Jalankan Aplikasi**: Klik dua kali pada `app.exe` untuk menjalankan aplikasi.
3. **Upload Data**: Di sidebar, upload file Excel untuk SO, Barang Masuk, dan Barang Keluar.
4. **Cleaning Data**: Pilih tab "Data Cleaning", pilih file, atur pengaturan kolom, dan simpan cleaning.
5. **Proses FIFO**: Pilih tab "Integrasi FIFO", map kolom, atur kolom tambahan jika perlu, lalu jalankan FIFO.
6. **Unduh Hasil**: Setelah proses selesai, unduh hasil sebagai file Excel.

## Catatan Penting

- Minimal data yang diperlukan: (SO + Keluar) atau (Masuk + Keluar).
- Pastikan mapping kolom wajib tidak kosong ('-').
- Aplikasi menggunakan logika FIFO untuk menghitung stok.

## Pengembang
Dibuat oleh **Nadiyatul Jenni**.
Menggunakan teknologi:
* [Streamlit](https://streamlit.io/) - Framework Antarmuka Pengguna
* [Pandas](https://pandas.pydata.org/) - Pengolahan Data
* [OpenPyXL](https://openpyxl.readthedocs.io/) - Manipulasi File Excel
