# Akuisisi Data Akomodasi di Kecamatan Kintamani

**Mata Kuliah:** BIFP-243 Akuisisi dan Manajemen Data
**Pengambil Data:** Ni Kadek Satya Giri Sardhula (NIM: 2501010088)
**Tanggal Akses (UTC):** 2026-11-11

## 1. Deskripsi Proyek
Mengumpulkan, meratakan, dan mendokumentasikan data akomodasi di Kecamatan Kintamani, Kabupaten Bangli, Bali secara etis.

## 2. Sumber Data & Atribusi
* **OpenStreetMap (Overpass API)**, berlisensi ODbL.
* **© OpenStreetMap contributors**.

## 3. Batasan Etika
* Mematuhi rate limit Overpass API.
* Minimisasi data: tidak mengambil telepon, email, dan akun media sosial pemilik.
* Tidak melakukan scraping platform OTA (Airbnb, Booking.com, Agoda, dll.).

## 4. Pembersihan Data
* Duplikat (osm_type + osm_id) dibuang.
* Objek di luar bounding box Kintamani dibuang dan disimpan terpisah.
* Objek tanpa nama dipertahankan.

## 5. Cara Menjalankan Ulang
1. Buka di Google Colab atau jalankan `python akuisisi_akomodasi_kintamani.py`.
2. Raw JSON di `data/raw/`, CSV bersih di `data/interim/akomodasi_kintamani.csv`.
3. Grafik dan peta (jika tersedia) di `reports/`.

## 6. Struktur Repositori
- `data/` : raw dan interim
- `docs/` : metadata dan dokumentasi
- `reports/` : laporan, grafik, peta
