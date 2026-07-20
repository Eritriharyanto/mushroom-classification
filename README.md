# 🍄 Mushroom Classification

Tugas UAS Mata Kuliah Pembelajaran Mesin — proyek *supervised machine learning* untuk mengklasifikasikan jamur ke dalam kategori **dapat dimakan (edible)** atau **beracun (poisonous)** berdasarkan ciri-ciri morfologinya (bentuk topi, warna, bau, habitat, dll).

## 📊 Dataset

Dataset yang digunakan berasal dari Kaggle:
[Mushroom Classification Dataset](https://www.kaggle.com/datasets/uciml/mushroom-classification)

### Informasi Atribut

| Atribut | Keterangan |
|---|---|
| `class` | Kelas target: edible = `e`, poisonous = `p` |
| `cap-shape` | Bentuk topi: bell=`b`, conical=`c`, convex=`x`, flat=`f`, knobbed=`k`, sunken=`s` |
| `cap-surface` | Permukaan topi: fibrous=`f`, grooves=`g`, scaly=`y`, smooth=`s` |
| `cap-color` | Warna topi: brown=`n`, buff=`b`, cinnamon=`c`, gray=`g`, green=`r`, pink=`p`, purple=`u`, red=`e`, white=`w`, yellow=`y` |
| `bruises` | Memar: bruises=`t`, no=`f` |
| `odor` | Bau: almond=`a`, anise=`l`, creosote=`c`, fishy=`y`, foul=`f`, musty=`m`, none=`n`, pungent=`p`, spicy=`s` |
| `gill-attachment` | Perlekatan insang: attached=`a`, descending=`d`, free=`f`, notched=`n` |
| `gill-spacing` | Jarak insang: close=`c`, crowded=`w`, distant=`d` |
| `gill-size` | Ukuran insang: broad=`b`, narrow=`n` |
| `gill-color` | Warna insang: black=`k`, brown=`n`, buff=`b`, chocolate=`h`, gray=`g`, green=`r`, orange=`o`, pink=`p`, purple=`u`, red=`e`, white=`w`, yellow=`y` |
| `stalk-shape` | Bentuk batang: enlarging=`e`, tapering=`t` |
| `stalk-root` | Akar batang: bulbous=`b`, club=`c`, cup=`u`, equal=`e`, rhizomorphs=`z`, rooted=`r`, missing=`?` |
| `stalk-surface-above-ring` | Permukaan batang di atas cincin: fibrous=`f`, scaly=`y`, silky=`k`, smooth=`s` |
| `stalk-surface-below-ring` | Permukaan batang di bawah cincin: fibrous=`f`, scaly=`y`, silky=`k`, smooth=`s` |
| `stalk-color-above-ring` | Warna batang di atas cincin: brown=`n`, buff=`b`, cinnamon=`c`, gray=`g`, orange=`o`, pink=`p`, red=`e`, white=`w`, yellow=`y` |
| `stalk-color-below-ring` | Warna batang di bawah cincin: brown=`n`, buff=`b`, cinnamon=`c`, gray=`g`, orange=`o`, pink=`p`, red=`e`, white=`w`, yellow=`y` |
| `veil-type` | Tipe selubung: partial=`p`, universal=`u` |
| `veil-color` | Warna selubung: brown=`n`, orange=`o`, white=`w`, yellow=`y` |
| `ring-number` | Jumlah cincin: none=`n`, one=`o`, two=`t` |
| `ring-type` | Tipe cincin: cobwebby=`c`, evanescent=`e`, flaring=`f`, large=`l`, none=`n`, pendant=`p`, sheathing=`s`, zone=`z` |
| `spore-print-color` | Warna cetakan spora: black=`k`, brown=`n`, buff=`b`, chocolate=`h`, green=`r`, orange=`o`, purple=`u`, white=`w`, yellow=`y` |
| `population` | Populasi: abundant=`a`, clustered=`c`, numerous=`n`, scattered=`s`, several=`v`, solitary=`y` |
| `habitat` | Habitat: grasses=`g`, leaves=`l`, meadows=`m`, paths=`p`, urban=`u`, waste=`w`, woods=`d` |

## 🎯 Tujuan

Membangun model klasifikasi yang mampu memprediksi apakah suatu jamur aman dikonsumsi atau beracun, berdasarkan fitur-fitur kategorikal di atas.

## 🧠 Model & Hasil

Dua algoritma *machine learning* digunakan dan dibandingkan performanya:

| Algoritma | Akurasi |
|---|---|
| Random Forest | **100%** |
| Logistic Regression | **96%** |

## 🛠️ Tahapan Analisis

1. **Import & instalasi library** yang dibutuhkan, di antaranya:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `scikit-learn` (`LabelEncoder`, `StandardScaler`, dll)
2. **Eksplorasi & pembersihan data** (Exploratory Data Analysis)
3. **Encoding** fitur kategorikal (Label Encoding)
4. **Standarisasi** fitur numerik (Standard Scaler)
5. **Split data** menjadi data latih dan data uji
6. **Pelatihan model** menggunakan Random Forest dan Logistic Regression
7. **Evaluasi model** menggunakan metrik akurasi, confusion matrix, dan classification report

## 📁 Struktur Repositori

```
mushroom-classification/
├── Jamur_2_model.ipynb   # Notebook analisis & pemodelan
└── README.md             # Dokumentasi proyek
```

## 🚀 Cara Menjalankan

1. Clone repositori ini:
   ```bash
   git clone https://github.com/Eritriharyanto/mushroom-classification.git
   cd mushroom-classification
   ```
2. Unduh dataset dari [Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification) dan letakkan pada direktori proyek.
3. Install dependensi yang dibutuhkan:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. Jalankan notebook `Jamur_2_model.ipynb` menggunakan Jupyter Notebook / Google Colab.

## 📌 Catatan

Proyek ini dibuat untuk memenuhi tugas Ujian Akhir Semester (UAS) mata kuliah **Pembelajaran Mesin**.

## 👤 Author

**Eritriharyanto**
