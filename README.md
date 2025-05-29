# Submission-Belajar_Fundamental-Deep-Learning_2

# Klasifikasi Gambar Indoherb

## Deskripsi

Proyek ini bertujuan untuk mengklasifikasikan gambar tanaman herbal di Indonesia menjadi 20 kelas berikut:

- Abelmoschus Esculentus (Okra)  
- Acorus Calamus (Dlingo)  
- Aloe Vera (Lidah Buaya)  
- Alstonia Scholaris (Pulai)  
- Amaranthus Spinosus (Bayam Duri)  
- Andrographis Paniculata (Sambiloto)  
- Annona Muricata (Sirsak)  
- Annona Squamosa (Srikaya)  
- Anredera Cordifolia (Binahong)  
- Apium Graveolens (Seledri)  
- Artocarpus Heterophyllus (Nangka Mini)  
- Artocarpus Integer (Nangka Cempedak)  
- Averrhoa Bilimbi (Belimbing Wuluh)  
- Blumea Balsamifera (Sembung)  
- Borreria Hispida (Gempur Batu)  
- Caesalpinia Sappan L (Secang)  
- Caladium Cicolor (Keladi)  
- Calendula Officinalis (Marigold)  
- Canangium Odoratum (Kenanga)  
- Catharanthus Roseus (Tapak Dara)  

Model yang digunakan adalah **MobileNetV2** dengan pendekatan **transfer learning** serta **data augmentation** untuk meningkatkan performa klasifikasi.

## Dataset

Dataset yang digunakan adalah *Indonesia-Medicinal-Plant-Dataset* dari Kaggle. Dataset ini berisi gambar-gambar tanaman herbal Indonesia dari berbagai kelas.

🔗 [Link ke dataset](https://www.kaggle.com/datasets/somilyadav999/indoherb)

## Langkah-langkah

1. **Persiapan Data**
   - Unduh dataset dari Kaggle.
   - Lakukan augmentasi data untuk semua kelas.
   - Bagi data menjadi training, validation, dan testing set.

2. **Pemodelan**
   - Gunakan **MobileNetV2** sebagai *base model*.
   - Tambahkan layer tambahan: Convolutional, MaxPooling, dan Dense.
   - Lakukan training model dengan data training.

3. **Evaluasi**
   - Evaluasi model menggunakan data testing dengan metrik akurasi.
   - Visualisasikan hasil evaluasi menggunakan **confusion matrix** dan **classification report**.

4. **Penyimpanan Model**
   - Simpan model dalam beberapa format:
     - Keras (`.keras`)
     - TensorFlow Lite (`.tflite`)
     - TensorFlow.js

## Cara Menjalankan

1. **Instalasi Library**

   Pastikan kamu telah menginstal semua dependensi yang diperlukan:
   ```bash
   pip install -r requirements.txt
2. **Jalankan notebook Jupyter:**
    - Buka file `notebook.ipynb` .
    - Jalankan semua sel kode secara berurutan.
