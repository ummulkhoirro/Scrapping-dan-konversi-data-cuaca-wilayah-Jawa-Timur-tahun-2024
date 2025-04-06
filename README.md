Proyek ini bertujuan untuk mengambil (scraping) data cuaca dari beberapa kota di Provinsi Jawa Timur menggunakan API dari OpenWeatherMap, lalu menyimpannya dalam berbagai format data terstruktur seperti CSV, JSON, dan Excel.

##  Deskripsi Proyek

Data cuaca dikumpulkan dari 20 kota di Jawa Timur seperti Surabaya, Malang, Kediri, Jember, dan lainnya. Informasi yang dikumpulkan meliputi:
- Nama Kota
- Suhu (dalam °C)
- Deskripsi Cuaca
- Kelembapan (%)
- Kecepatan Angin (m/s)
- Tanggal dan Waktu pengambilan data

Seluruh data yang awalnya berbentuk semi-terstruktur (JSON) akan dikonversi menjadi data terstruktur (tabular) dan disimpan ke dalam file CSV dan Excel.

## Tools & Library

- `Python`
- `requests`
- `pandas`
- `json`
- `BeautifulSoup` *(opsional, jika mengambil dari HTML)*
- API: [OpenWeatherMap API](https://openweathermap.org/api)

##  Struktur Output

- `cuaca_jawa_timur_2024.csv` — Data cuaca dalam format CSV
- `data_cuaca_jawa_timur.xlsx` — Data cuaca dalam format Excel
- JSON Pretty Print di console (opsional untuk visualisasi)

##  Cara Menjalankan

1. Pastikan sudah menginstall `requests` dan `pandas`:
    ```bash
    pip install requests pandas
    ```

2. Jalankan skrip Python yang disediakan:
    ```bash
    python cuaca_jawa_timur.py
    ```

3. Output akan tampil di terminal dan disimpan dalam file:
    - `cuaca_jawa_timur_2024.csv`
    - `data_cuaca_jawa_timur.xlsx`

> ⚠️ **Catatan**: Gantilah `API_KEY` pada skrip dengan API key pribadi Anda dari [OpenWeatherMap](https://home.openweathermap.org/users/sign_up).

## Daftar Kota yang Discrape

- Surabaya
- Malang
- Kediri
- Jember
- Mojokerto
- Probolinggo
- Banyuwangi
- Pasuruan
- Lumajang
- Sidoarjo
- Blitar
- Tulungagung
- Trenggalek
- Ngawi
- Magetan
- Pacitan
- Bondowoso
- Situbondo
- Jombang
- Madiun

## Tujuan Pembelajaran

Proyek ini cocok sebagai latihan untuk:
- Mengakses API publik
- Memproses data semi-terstruktur (JSON)
- Menyimpan data ke dalam berbagai format
- Konversi data menjadi bentuk yang mudah dianalisis

