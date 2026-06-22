# 🚕 Analisis Sentimen Ulasan Gojek vs Grab (Domain: Bisnis & Transportasi)

Proyek ini dibuat untuk memenuhi tugas besar mata kuliah NLP (Natural Language Processing). Fokus proyek ini adalah melakukan scraping data ulasan aplikasi Gojek dan Grab dari Google Play Store, melakukan analisis sentimen menggunakan dua pendekatan model (Klasik/RNN vs Transformer), dan mendeploy hasilnya ke Hugging Face Spaces menggunakan Streamlit.

---

## 📌 Ketentuan Utama Proyek
* **Target Dataset:** Minimal 10.000 data ulasan Bahasa Indonesia (gabungan Gojek & Grab).
* **Teknologi Model:** 
  1. Deep Learning Tradisional (LSTM / GRU)
  2. Transformer Modern (IndoBERT / HuggingFace)
* **Output Akhir:** Prototype aplikasi berbasis web yang sudah di-deploy.

---
```markdown
## 📂 Struktur Folder Proyek

```text
NLP_UAS/
├── data/
│   ├── raw/                  <- Simpan hasil scraping mentah di sini (Format .csv)
│   └── processed/            <- Simpan data setelah preprocessing & labeling di sini
├── notebooks/
│   ├── 01_scraping.ipynb      <- Anggota 1: Bagian penarikan data dari Play Store
│   ├── 02_preprocessing.ipynb <- Anggota 2: Pembersihan teks (case folding, stemming, dll)
│   ├── 03_model_lstm.ipynb   <- Anggota 3: Training model LSTM/GRU (TensorFlow)
│   └── 04_model_bert.ipynb   <- Anggota 4: Fine-tuning model IndoBERT (HuggingFace)
├── models/                   <- Folder untuk menyimpan file model yang sudah dilatih (.h5 / .pt)
│   ├── lstm_model/
│   └── indobert_model/
├── reports/                  <- Grafik akurasi, Confusion Matrix, dan draf laporan PDF
│   └── figures/
├── app.py                    <- Script UI/Aplikasi web menggunakan Streamlit
├── requirements.txt          <- Daftar library Python yang digunakan
└── README.md                 <- Dokumentasi utama proyek (File ini)

---