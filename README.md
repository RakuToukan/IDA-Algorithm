# Implementasi Algoritma Iterative Deepening A* (IDA*)

![Visualisasi Graf](GrafAmerika.png)

Repositori ini berisi implementasi algoritma **Iterative Deepening A* (IDA*)** untuk mencari rute terpendek antar kota. Proyek ini mendemonstrasikan bagaimana IDA* bekerja secara efisien dalam mengelola memori namun tetap memberikan hasil yang optimal.

## 📋 Tentang Algoritma
IDA* (Iterative Deepening A*) adalah algoritma pencarian yang menggabungkan strategi *Depth-First Search* (DFS) dengan keuntungan dari fungsi heuristik *A** search. 

**Karakteristik Utama:**
- **Fungsi Heuristik ($f(n) = g(n) + h(n)$):** Digunakan untuk mengestimasi biaya total dari titik awal ke tujuan.
- **Threshold (Ambang Batas):** IDA* menggunakan batas biaya untuk membatasi pencarian DFS. Jika solusi tidak ditemukan, batas ini akan ditingkatkan berdasarkan nilai biaya terkecil yang melebihi ambang sebelumnya.
- **Efisiensi Memori:** Sangat hemat memori dibandingkan A* karena tidak menyimpan semua *node* yang dikunjungi.

## 📍 Kasus Studi: Rute STL ke SSM
Dalam implementasi ini, program mencari jalur optimal dari **Saint Louis (STL)** menuju **Sault Ste. Marie (SSM)**.

**Hasil Pencarian:**
- **Path:** `STL -> KCY -> OMA -> DLH -> SSM`
- **Total Cost:** 320

## 🚀 Fitur Utama
- **Algoritma IDA* Murni:** Implementasi fungsi rekursif dengan *thresholding*.
- **Visualisasi Graf:** Menggunakan `NetworkX` dan `Matplotlib` untuk menampilkan keterhubungan antar kota dan bobot jalurnya.
- **Visualisasi Jalur:** Node yang terpilih sebagai jalur utama akan diberi warna berbeda (Hijau) agar mudah dibedakan.

## 🛠️ Persiapan Lingkungan
1. Pastikan Python 3.x telah terinstal.
2. Instal library yang dibutuhkan:
   ```bash
   pip install networkx matplotlib numpy

Credit :
1. [@Jetluck](https://github.com/r6rap) - Algoritma IDA*
2. [@Raku](https://github.com/RakuToukan) - Dokumentasi & Visualisasi Graf
