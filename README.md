# 🌱 Smart Farming IoT Data Analysis Dashboard

## 📌 Project Overview

Project ini bertujuan untuk memonitor dan menganalisis **kelembaban tanah** menggunakan data sensor IoT dalam sistem **Smart Farming**.  
Dashboard interaktif dibuat menggunakan **Streamlit** untuk memvisualisasikan kondisi tanah, tren kelembaban, korelasi antar sensor, dan aktivitas irigasi.

## 📂 Dataset

Dataset berisi data sensor kelembaban tanah dengan atribut:

- `year`, `month`, `day`, `hour`, `minute`, `second`
- `moisture0` – `moisture4` (data kelembaban dari sensor 1–5)
- `irrgation` (status irigasi)

### Preprocessing

Data diproses dengan langkah-langkah berikut:

1. Menghapus missing values
2. Membersihkan data sensor
3. Menyimpan dataset bersih menjadi `cleaned_data.csv`

### Data Quality Metrics

Kualitas data diukur dengan tiga metrik:

- **Accuracy**: `1 - (missing / total)`
- **Completeness**: `non-null / total cells`
- **Timeliness**: persentase data terbaru dalam 30 hari terakhir

---

## 🖥 Dashboard Features

Dashboard menampilkan:

1. **Current, Average, Max Moisture** – Metrik kelembaban sensor saat ini
2. **Soil Moisture Trend** – Grafik line chart tren kelembaban
3. **Moisture Distribution** – Histogram distribusi kelembaban
4. **Sensor Correlation** – Heatmap korelasi antar sensor
5. **Irrigation Activity** – Aktivitas irigasi harian
6. **Soil Moisture Alert** – Notifikasi kondisi tanah (kering / normal)

### Teknologi yang Digunakan

- **Python 3.x**
- **Streamlit**
- **Pandas**
- **Matplotlib**
- **Seaborn**

---

## 🚀 How to Run Dashboard

1. Install dependencies:

```bash
pip install streamlit pandas matplotlib seaborn
```
