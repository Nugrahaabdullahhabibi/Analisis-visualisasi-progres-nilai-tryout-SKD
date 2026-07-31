# SKD Progress Tracker & Analyzer

<div align="center">

<img src="Anilisi-visualisasi-uji coba-SKD" width="100%">

</div>

---

Analisis dan visualisasi progres nilai tryout SKD (Seleksi Kompetensi Dasar), dibangun dengan Python (Pandas, Matplotlib & Plotly).

## Latar Belakang
# SKD Progress Tracker & Analyzer

Analisis dan visualisasi progres nilai tryout SKD (Seleksi Kompetensi Dasar), dibangun dengan Python (Pandas, Matplotlib, Plotly).

## Latar Belakang

Sebagai bagian dari persiapan mengikuti seleksi Sekolah Kedinasan, saya rutin mengerjakan tryout SKD (TWK, TIU, TKP) untuk mengukur kesiapan diri saya. Alih-alih hanya mencatat nilai secara manual, saya membangun tools sederhana untuk melacak progres, memvisualisasikan tren, dan menganalisis komponen mana yang perlu diperkuat sekaligus sebagai latihan praktis skill data analysis.

## Tujuan Projek

- Melacak progres nilai TWK, TIU, TKP dari waktu ke waktu
- Mengidentifikasi komponen yang paling sering di bawah passing grade
- Melihat tren perkembangan nilai secara keseluruhan
- Membangun dashboard interaktif untuk eksplorasi data yang lebih mudah

## Tools & Library

- **Python** — bahasa utama
- **Pandas** — pembacaan & pembersihan data dari Excel
- **Matplotlib** — visualisasi statis (line chart, bar chart, pie chart)
- **Plotly** — dashboard interaktif (hover, zoom)
- **NumPy** — perhitungan tren (regresi linear sederhana)

## Alur Analisis

1. **Data Foundation** — mengumpulkan nilai tryout ke dalam file Excel terstruktur (No, Nama Tryout, Tanggal, TWK, TIU, TKP, Total Score)
2. **Visualisasi Dasar** — line chart progres nilai, bar chart perbandingan per komponen dengan garis passing grade
3. **Analisis & Insight** — statistik ringkas, frekuensi nilai di bawah passing grade, tren naik/turun, korelasi antar komponen
4. **Dashboard Interaktif** — versi Plotly dari seluruh visualisasi agar bisa di-hover dan dieksplorasi lebih detail

## Insight yang Ditemukan

- Dari 31 tryout yang dikerjakan, komponen **TWK** hanya 1 kali berada di bawah passing grade, sementara **TIU** dan **TKP** konsisten selalu lolos.
- Berdasarkan ambang nilai total ≥420, mayoritas tryout berada di kategori "Aman".
- Tren nilai total menunjukkan kecenderungan **naik** seiring bertambahnya jumlah tryout yang dikerjakan.

## Cara Menjalankan

1. Clone repository ini
2. Install dependencies:
   ```bash
   pip install pandas matplotlib plotly openpyxl
   ```
3. Buka `StastistikSKD.ipynb` di Jupyter Notebook / JupyterLab
4. Jalankan seluruh cell secara berurutan (Run → Run All Cells)

## Struktur File

```
├── StastistikSKD.ipynb      # Notebook utama analisis
├── DATA_TRYOUT.xlsx         # Data nilai tryout
└── README.md                # Dokumentasi projek
```

## Rencana Pengembangan

- [ ] Analisis lebih dalam per sub-topik soal (misal: soal cerita vs hitungan di TIU)
- [ ] Prediksi nilai tryout berikutnya berdasarkan tren
- [ ] Deploy dashboard sebagai web app menggunakan Streamlit

---

*Proyek personal untuk mendukung persiapan seleksi Sekolah Kedinasan, sekaligus latihan penerapan data analysis di kasus nyata.*
