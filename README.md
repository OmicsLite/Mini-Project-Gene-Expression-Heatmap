# Mini-Project-Gene-Expression-Heatmap
Menganalisis pola ekspresi gen pada beberapa sampel biologis dan memvisualisasikan perbedaannya menggunakan heatmap.



## Gambaran Umum

Proyek ini bertujuan untuk mengeksplorasi pola ekspresi gen pada jaringan payudara normal dan sampel tumor payudara menggunakan Python.

Analisis ini menggunakan dataset microarray publik **GSE29431** yang tersedia di NCBI Gene Expression Omnibus (GEO).

Untuk menghasilkan visualisasi dengan jumlah sampel yang seimbang, analisis ini menggunakan 12 sampel jaringan normal dan 12 sampel tumor yang dipilih secara acak.

## Pertanyaan Penelitian

Bagaimana perbedaan pola ekspresi gen antara jaringan payudara normal dan jaringan tumor payudara?

## Informasi Dataset

- **GEO Accession:** GSE29431
- **Organisme:** Homo sapiens
- **Platform:** GPL570 (Affymetrix Human Genome U133 Plus 2.0 Array)
- **Jumlah sampel asli:** 66
- **Jumlah sampel normal asli:** 12
- **Jumlah sampel tumor asli:** 54
- **Sampel normal yang dipilih:** 6
- **Sampel tumor yang dipilih:** 6
- **Total sampel yang dianalisis:** 12

Sumber dataset: https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE29431

## Tools dan Library

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Metodologi

Tahapan analisis dalam proyek ini meliputi:

1. Mengunduh dataset GSE29431 dari NCBI GEO.
2. Memuat matriks ekspresi gen dan metadata sampel.
3. Mengidentifikasi sampel jaringan normal dan tumor.
4. Memilih 6 sampel normal dan 6 sampel tumor secara acak.
5. Melakukan prapemrosesan data dasar.
6. Mengeksplorasi distribusi ekspresi gen.
7. Memilih 30 probe set dengan variasi ekspresi tertinggi.
8. Melakukan standardisasi Z-score antar sampel.
9. Membuat heatmap dengan hierarchical clustering.
10. Menginterpretasikan pola ekspresi gen yang dihasilkan.

## Interpretasi

Heatmap digunakan untuk memvisualisasikan pola ekspresi relatif gen pada sampel jaringan normal dan tumor yang telah dipilih.

Warna merah menunjukkan tingkat ekspresi yang relatif lebih tinggi, sedangkan warna biru menunjukkan tingkat ekspresi yang relatif lebih rendah setelah standardisasi Z-score.

Hierarchical clustering mengelompokkan sampel berdasarkan kemiripan pola ekspresi gennya.

Dengan visualisasi ini, kita dapat mengeksplorasi apakah sampel jaringan normal dan tumor memiliki pola ekspresi gen yang berbeda.

## Catatan Penting

Subset sampel yang seimbang dalam proyek ini digunakan untuk keperluan visualisasi eksploratif dan pembelajaran.

Pemilihan 6 sampel tumor secara acak tidak sepenuhnya merepresentasikan seluruh variasi biologis dari 54 sampel tumor yang tersedia dalam dataset asli.

Heatmap saja tidak dapat membuktikan signifikansi statistik ataupun mengidentifikasi biomarker kanker yang telah tervalidasi.

Analisis lanjutan, seperti *differential expression analysis* dan validasi biologis, diperlukan untuk mengidentifikasi gen yang memiliki perbedaan ekspresi secara signifikan serta memahami relevansi biologisnya.

## Cara Menjalankan Proyek

1. Buka notebook melalui Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LNiPgABLCZHk5_fJs-T9-s6OZ6g2E6wA)
2. Jalankan setiap sel kode secara berurutan.
3. Dataset akan diunduh secara otomatis dari NCBI GEO.
4. Amati visualisasi dan hasil analisis yang dihasilkan.

## Referensi

NCBI Gene Expression Omnibus (GEO). GSE29431: Identifying Breast Cancer Biomarkers.

https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE29431

---

**Dikembangkan oleh OmicsLite**
