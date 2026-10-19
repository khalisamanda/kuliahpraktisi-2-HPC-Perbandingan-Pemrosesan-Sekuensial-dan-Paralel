# Implementasi High Performance Computing untuk Perbandingan Pemrosesan Sekuensial dan Paralel

## Ringkasan

Proyek ini membandingkan waktu pemrosesan data kualitas udara menggunakan pendekatan sekuensial dan paralel. Tujuannya adalah memahami bagaimana pembagian pekerjaan ke beberapa proses dapat memengaruhi waktu komputasi dan kesetaraan hasil.

## Dataset

- **Nama:** Air Quality
- **Sumber resmi:** UCI Machine Learning Repository
- **Halaman dataset:** https://archive.ics.uci.edu/dataset/360/air+quality
- **Jumlah observasi:** 9.358 pengukuran
- **Jenis data:** Pengukuran kualitas udara per jam dari sensor kimia di sebuah kota di Italia.

Notebook mengambil dataset dari sumber publik, melakukan pembersihan awal, kemudian menggunakan data numerik tersebut sebagai beban pemrosesan.

## Tujuan

1. Memuat dan memeriksa data kualitas udara.
2. Menangani nilai khusus yang menandakan data hilang.
3. Menyiapkan operasi numerik untuk pengujian komputasi.
4. Membandingkan waktu pemrosesan sekuensial dan paralel.
5. Memastikan kedua pendekatan menghasilkan keluaran yang setara.
6. Menghitung perbedaan waktu dan percepatan pemrosesan (*speedup*).

## Metode dan metrik

- Pemeriksaan dan pembersihan data.
- Operasi numerik menggunakan NumPy.
- Pemrosesan sekuensial sebagai baseline.
- Pemrosesan paralel menggunakan multiprocessing.
- Pengukuran waktu dengan timer.
- Perbandingan waktu eksekusi.
- Perhitungan speedup dan pemeriksaan kesetaraan hasil.

## Batasan dan penggunaan yang bertanggung jawab

- Pengujian di Google Colab merupakan demonstrasi komputasi paralel, bukan benchmark superkomputer profesional.
- Waktu eksekusi dapat dipengaruhi jumlah CPU, beban server, ukuran data, dan overhead pembuatan proses.
- Data yang diulang untuk menambah beban komputasi tidak boleh dianggap sebagai observasi baru.
- Pemrosesan paralel tidak selalu lebih cepat untuk pekerjaan kecil.
- Kesimpulan akhir harus berdasarkan waktu yang benar-benar diukur saat notebook dijalankan.
