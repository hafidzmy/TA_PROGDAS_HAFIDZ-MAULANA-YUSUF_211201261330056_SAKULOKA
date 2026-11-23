# Aplikasi Pengelolaan Keuangan Pribadi Mahasiswa

Aplikasi desktop sederhana berbasis Python dan Tkinter untuk mencatat pemasukan, pengeluaran, anggaran, serta laporan keuangan.

## Fitur
- Dashboard saldo, pemasukan dan pengeluaran bulan berjalan.
- Tambah, edit, hapus, cari, dan filter transaksi.
- Anggaran bulanan dan anggaran per kategori.
- Laporan bulanan dan ekspor transaksi ke CSV.
- Penyimpanan lokal otomatis menggunakan JSON.

## Persyaratan
- Python 3.9 atau lebih baru.
- Tkinter (umumnya sudah disertakan pada instalasi Python desktop).
- Tidak membutuhkan library eksternal.

## Cara menjalankan
1. Ekstrak folder proyek.
2. Buka terminal/Command Prompt pada folder `Aplikasi_Keuangan_Mahasiswa`.
3. Jalankan dengan salah satu cara berikut:

   - Windows: klik dua kali `Jalankan_Aplikasi.bat`, atau jalankan perintah di bawah.
   - Terminal: jalankan:

   ```bash
   python main.py
   ```

   Pada beberapa perangkat, gunakan `python3 main.py`.

4. Data transaksi akan tersimpan otomatis pada `data_keuangan.json` di folder proyek.

## Format pengisian
- Nominal diisi dengan angka rupiah tanpa desimal, misalnya `25000` atau `25.000`.
- Tanggal menggunakan format `YYYY-MM-DD`, misalnya `2026-11-22`.
- Filter laporan menggunakan format `YYYY-MM`, misalnya `2026-11`.

## Struktur file
- `main.py`: menjalankan aplikasi.
- `gui.py`: tampilan Tkinter dan interaksi pengguna.
- `models.py`: class Transaksi, Pemasukan, Pengeluaran, dan Anggaran.
- `pengelola_keuangan.py`: proses transaksi, saldo, anggaran, dan laporan.
- `penyimpanan.py`: baca/tulis data JSON.
- `data_keuangan.json`: penyimpanan data lokal.

## Catatan
Saldo adalah akumulasi seluruh pemasukan dikurangi seluruh pengeluaran yang tercatat. Ringkasan pemasukan dan pengeluaran pada dashboard dihitung untuk bulan berjalan. Aplikasi ini merupakan proyek praktikum; data hanya tersimpan secara lokal pada komputer tempat aplikasi dijalankan.
