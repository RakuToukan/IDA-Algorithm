# Implementasi Algoritma Iterative Deepening A* (IDA*) - Penentuan Rute Terpendek

Proyek ini merupakan implementasi algoritma **Iterative Deepening A* (IDA*)** untuk mencari rute terpendek antar lokasi di wilayah Jawa Timur (khususnya sekitar Gedangan, Waru, dan Surabaya). Proyek ini disusun sebagai bagian dari tugas mata kuliah Kecerdasan Buatan (AI).

## 📋 Deskripsi Proyek
IDA* adalah algoritma pencarian grafik yang menggabungkan strategi *Depth-First Search* (DFS) dengan keuntungan dari fungsi heuristik *A** search. Berbeda dengan A*, IDA* menggunakan ruang memori yang jauh lebih sedikit karena beroperasi seperti DFS namun tetap menjamin solusi optimal.

Dalam proyek ini, kami memodelkan beberapa titik lokasi sebagai *nodes* dan jalan antar lokasi sebagai *edges* dengan bobot jarak.

## 📍 Peta Lokasi (Graf)
Kami menggunakan data lokasi koordinat asli untuk menghitung jarak antar titik menggunakan formula Haversine/Euclidean. Titik-titik yang digunakan meliputi:
- Gedangan (GDN)
- Waru Barat (WRB) & Waru Timur (WRT)
- Gayungan (GYN)
- Sedati (SDT)
- Gunung Anyar (GNY)
- Rungkut (RKT)
- Tenggilis Mejoyo (TGY)

![Visualisasi Graf](GrafAmerika.png) 
*(Catatan: Pastikan nama file gambar di repo sesuai dengan `Graf Amerika.png`)*

## 🚀 Fitur Utama
- **Representasi Graf:** Menggunakan `NetworkX` untuk manajemen struktur data node dan edge.
- **Fungsi Heuristik:** Menggunakan jarak garis lurus (Straight-Line Distance) antar koordinat sebagai estimasi biaya menuju tujuan.
- **Visualisasi Interaktif:** Menggunakan `Folium` untuk menampilkan rute hasil pencarian di atas peta digital (OpenStreetMap).
- **Analisis Performa:** Menghitung total biaya (jarak) dan membandingkan rute yang dihasilkan.

## 🛠️ Teknologi yang Digunakan
- **Python 3.x**
- **Library:**
  - `NetworkX` (Struktur Graf)
  - `Folium` (Visualisasi Peta)
  - `Matplotlib` (Plotting)
  - `Math` & `Geopy` (Perhitungan Jarak)

## 📖 Cara Penggunaan
1. Pastikan Anda memiliki lingkungan Python yang sudah terinstal.
2. Instal dependensi yang diperlukan:
   ```bash
   pip install networkx matplotlib folium
