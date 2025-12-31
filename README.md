# PKM-TULIP: Sistem Pemantauan Interaktif Kualitas Udara dan Radiasi Berbasis IoT

![Status](https://img.shields.io/badge/Status-Prototype-green) ![Platform](https://img.shields.io/badge/Platform-ESP32%20%7C%20Web-blue)

## 📖 Deskripsi Proyek
**PKM-TULIP** adalah solusi pemantauan lingkungan terintegrasi yang diusulkan dalam **Pekan Kreativitas Mahasiswa (PKM) 2025**. Sistem ini dirancang untuk memantau **kualitas udara** dan **tingkat radiasi lingkungan** secara *real-time* sebagai sarana edukasi nuklir bagi masyarakat.

Sistem bekerja dengan mengukur parameter lingkungan menggunakan sensor, mengirimkan data melalui komunikasi jarak jauh LoRa, dan menampilkannya pada dashboard web interaktif.

## 🚀 Fitur Utama
* **Multi-Sensor Monitoring:** Mendeteksi Gas CO, Suhu, Kelembaban, Tekanan Udara, dan Radiasi Gamma.
* **Komunikasi LoRa:** Pengiriman data jarak jauh (433MHz) dari titik pantau ke *gateway* internet.
* **Edukasi Nuklir:** Visualisasi tingkat radiasi yang mudah dipahami (aman/bahaya).
* **Dashboard Web:** Tampilan grafik *real-time* yang dapat diakses via browser.

## 🛠️ Komponen & Hardware
[cite_start]Daftar komponen utama yang digunakan dalam proyek ini [cite: 415-484]:
* **Mikrokontroler:** ESP32 DevKitC V4 (WiFi + Bluetooth).
* **Sensor Udara:** MQ-7 (Karbon Monoksida) & MQ-135.
* **Sensor Lingkungan:** DHT22 (Suhu/Kelembaban) & BMP280 (Tekanan Udara).
* **Detektor Radiasi:** Geiger Counter Kit (Miller Tube GM Tube Kamjay).
* **Posisi:** GPS NEO-7M.
* **Komunikasi:** Modul LoRa Ra-02 SX1278 (433MHz).
* **Power:** Solar Panel 8x11, Baterai 18650, Modul TP4056, MT3608 Step Up.

## 📂 Struktur Folder
* `/firmware`: Kode program untuk ESP32 (Transmitter & Receiver).
* `/web-dashboard`: Kode HTML/CSS/JS untuk tampilan antarmuka pengguna.
* `/docs`: Dokumentasi proyek termasuk Proposal PKM.

## 👥 Tim Pengembang (Kelompok 1)
Proyek ini dikembangkan oleh mahasiswa **Politeknik Teknologi Nuklir Indonesia - BRIN Yogyakarta**:

1.  **Muhammad Meisandi Baihaqi** (Ketua)
2.  Nashwa Lu'lu' Muthmainnah
3.  Fara Ulvia
4.  Gilas Gethar Prawoto
5.  Dimas Darmansyah
*(Beserta anggota tim Himpunan Mahasiswa Einsten.com lainnya)*

---
*Proyek ini diajukan untuk Pekan Kreativitas Mahasiswa (PKM) Tahun 2025.*
