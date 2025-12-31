<div align="center">

  <img src="https://via.placeholder.com/150?text=PKM+TULIP" alt="Logo Placeholder" width="150" height="150">

  # PKM-TULIP: Smart Radiation & Air Quality Monitoring
  
  **Sistem Pemantauan Interaktif Kualitas Udara dan Radiasi Berbasis IoT untuk Edukasi Nuklir**

  ![Platform](https://img.shields.io/badge/Platform-ESP32-blue?style=for-the-badge&logo=espressif)
  ![Communication](https://img.shields.io/badge/Comms-LoRa%20433MHz-red?style=for-the-badge)
  ![Status](https://img.shields.io/badge/Status-Prototype-green?style=for-the-badge)
  ![License](https://img.shields.io/badge/License-MIT-orange?style=for-the-badge)

</div>

---

## 📋 Ikhtisar (Overview)

**PKM-TULIP** adalah inovasi teknologi pemantauan lingkungan yang menggabungkan deteksi radiasi nuklir dan polusi udara dalam satu perangkat mandiri. Proyek ini dikembangkan untuk **Pekan Kreativitas Mahasiswa (PKM) 2025** dengan tujuan meningkatkan literasi nuklir masyarakat melalui data yang transparan.

### 🌟 Fitur Unggulan
- **Dual Monitoring:** Deteksi dini bahaya radiasi Gamma dan gas Karbon Monoksida (CO).
- **Long Range Telemetry:** Menggunakan modul LoRa SX1278 untuk pengiriman data jarak jauh (tanpa internet di node sensor).
- **Interactive Dashboard:** Visualisasi data *real-time* berbasis web yang mudah diakses.
- **Independent Power:** Ditenagai baterai 18650 dengan sistem pengisian panel surya.

---

## 🏗️ Alur Sistem

Data dikumpulkan dari sensor lapangan dan dikirimkan ke server untuk ditampilkan ke masyarakat.

```mermaid
graph LR
    A[Node Sensor] -->|LoRa 433MHz| B[Gateway ESP32]
    B -->|WiFi| C[ThingSpeak Cloud]
    C -->|API| D[Web Dashboard]
    D -->|Akses| E[Masyarakat/User]
