# README — Pemodelan Topik Berita Indonesia (LSA, NMF, LDA, BERTopic)

Dokumen ini menjelaskan langkah-langkah untuk menyiapkan lingkungan, mengunduh dataset, serta menjalankan kode yang digunakan dalam proyek pemodelan topik berita berbahasa Indonesia. Proyek ini memisahkan alur menjadi dua bagian utama:

1. **Preprocessing** — pembersihan teks hingga stemming (UAS NLP 1.0.ipynb).
2. **Modelling & Visualisasi** — pemodelan topik (LSA, NMF, LDA, BERTopic), evaluasi, dan visualisasi (UAS NLP 2.0.ipynb).

---

## Mengunduh Dataset

Pada proyek ini dataset utama berasal dari Kaggle:  
`https://www.kaggle.com/datasets/iqbalmaulana/indonesian-news-dataset`

### Menggunakan Kaggle Hub

Run Kode berikut

```Python
import kagglehub
import pandas as pd

path = kagglehub.dataset_download("iqbalmaulana/indonesian-news-dataset")
print("Path to dataset files:", path)

df = os.path.join(path, "data.csv")
```

## Requirements

```Requirements
bertopic[all]
gensim
hdbscan
matplotlib
numpy
pandas
pyLDAvis
sastrawi
scikit-learn
sentence-transformers
seaborn
spacy==3.5.0
Sastrawi
tqdm
umap-learn
```

## Cara menjalankan notebook/script

1. Buka file **"UAS NLP 1.0.ipynb"** dan run kode tersebut hingga mengghasilkan file **"stemmed_data.csv"**.
2. Jalankan kode **"UAS NLP 2.0.ipynb"** untuk model, visualisasi dan metriks evaluasi.
# indonesian-news-multimodel-topic-analysis
