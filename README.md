
## 📊 Analisis MANOVA pada Dataset Adult Income

Proyek ini merupakan implementasi **Multivariate Analysis of Variance (MANOVA)** untuk menganalisis pengaruh variabel demografis terhadap indikator ekonomi berdasarkan data *Adult Income* dari UCI Machine Learning Repository.

### 🔍 Tujuan

Mengetahui apakah terdapat perbedaan **pendapat** dan **pekerjaan** berdasarkan kategori variabel **capital.gain**, dan **capital.loss**.

### 🧪 Metode Analisis

**Multivariate Analysis of Variance (MANOVA)** digunakan untuk:

* Menguji pengaruh simultan variabel independen kategorik terhadap dua variabel dependen numerik.
* Mengidentifikasi variabel demografis yang secara signifikan memengaruhi **capital.gain** dan **capital.loss**.

### 🗂 Dataset

* **Sumber**: [UCI Machine Learning Repository – Adult Data](https://archive.ics.uci.edu/ml/datasets/adult)
* **Jumlah Data**: ±32.000 entri
* **Variabel Dependen**: `capital.gain`, `capital.loss`
* **Variabel Independen**: `income`, `occupation`

### 🛠 Teknologi yang Digunakan

* **Bahasa**: R
* **Tools/Pustaka**:

  * `tidyverse` – manipulasi data
  * `psych` – statistik deskriptif
  * `car` – uji MANOVA
  * `GGally`, `corrplot` – visualisasi hubungan antar variabel

### 📄 Isi Skrip

File `Script Metode MANOVA.Rmd` mencakup tahapan berikut:

1. **Data Cleaning & Encoding**
2. **Eksplorasi Statistik Deskriptif**
3. **Uji Asumsi MANOVA** (normalitas, homogenitas kovarian)
4. **Uji MANOVA** – Analisis pengaruh `income`, `occupation` terhadap `capital.gain` & `capital.loss`
5. **Interpretasi Hasil Uji** (Wilks’ Lambda, Pillai's Trace, dsb.)

### 📌 Output Penting

* Uji MANOVA menunjukkan perbedaan signifikan berdasarkan faktor demografis.
* Analisis dilengkapi visualisasi distribusi dan korelasi antar variabel.
