
# Penerapan Transfer Learning dengan Kombinasi Arsitektur VGGNet dan MobileNet untuk Klasifikasi Kanker Kulit

Proyek ini bertujuan untuk mengembangkan model deep learning yang dapat mengklasifikasikan gambar kanker kulit menggunakan pendekatan **Transfer Learning**. Model ini memanfaatkan dua arsitektur deep learning terkenal, **VGGNet** dan **MobileNet**, untuk mendeteksi dan mengklasifikasikan jenis-jenis kanker kulit berdasarkan citra medis.

## Deskripsi Proyek

Dalam penelitian ini, digunakan pendekatan **Transfer Learning** untuk melakukan klasifikasi jenis-jenis kanker kulit, termasuk:
- **Basal Cell Carcinoma** (BCC)
- **Squamous Cell Carcinoma** (SCC)
- **Melanoma**
- **Actinic Keratosis** (AK)

Transfer learning dilakukan dengan memanfaatkan arsitektur jaringan yang telah dilatih sebelumnya, seperti **VGGNet** dan **MobileNet**, yang kemudian disesuaikan untuk klasifikasi kanker kulit.

## Fitur Utama

- **Transfer Learning** dengan arsitektur **VGGNet** dan **MobileNet**.
- Evaluasi model menggunakan metrik seperti **accuracy**, **precision**, **recall**, **F1-score**, dan **AUC**.
- Visualisasi hasil eksperimen dan metrik evaluasi.
- Penyimpanan model terbaik dan visualisasi hasil.

## Instalasi

### Persyaratan

Sebelum menjalankan proyek ini, pastikan bahwa Anda telah menginstal semua dependensi yang diperlukan. Anda dapat menginstal dependensi menggunakan `pip` dengan menjalankan perintah berikut:

```bash
pip install -r requirements.txt
```

### Cara Menjalankan Proyek

1. Clone repositori ini ke direktori lokal Anda:
   ```bash
   git clone https://github.com/username/repository-name.git
   cd repository-name
   ```

2. Setelah itu, instal dependensi yang dibutuhkan:
   ```bash
   pip install -r requirements.txt
   ```

3. Siapkan dataset gambar kanker kulit dalam folder yang terpisah berdasarkan kelas kanker kulit (misalnya, BCC, SCC, Melanoma, AK).

4. Jalankan skrip utama untuk memulai pelatihan model:
   ```bash
   python src/trainer.py
   ```

## Struktur Direktori

```
project-folder/
│
├── data/                # Folder untuk dataset gambar kanker kulit
├── models/              # Folder untuk menyimpan model yang telah dilatih
│   └── checkpoints/     # Penyimpanan model terbaik
├── results/             # Folder untuk hasil eksperimen dan visualisasi
│   ├── logs/            # Log eksperimen
│   └── visualizations/  # Hasil visualisasi
├── src/                 # Sumber kode utama
│   ├── data_processor.py    # Kode untuk memproses data
│   ├── model.py            # Definisi model
│   └── trainer.py          # Proses pelatihan dan evaluasi model
├── README.md            # Dokumentasi proyek
└── requirements.txt      # Daftar dependensi
```

## Langkah-langkah Penggunaan

1. **Memproses Data**:
   - Siapkan dataset gambar kanker kulit dalam format yang sesuai. Dataset ini harus terdiri dari beberapa folder, masing-masing mewakili jenis kanker kulit (misalnya, BCC, SCC, Melanoma, AK).
   
2. **Menyiapkan Model**:
   - Proyek ini menggunakan arsitektur **VGGNet** dan **MobileNet** yang telah dilatih sebelumnya.
   - Model akan dilatih menggunakan dataset yang disediakan dan dievaluasi menggunakan metrik yang relevan.

3. **Pelatihan Model**:
   - Jalankan skrip pelatihan untuk melatih model dengan data yang ada.
   - Selama pelatihan, log eksperimen akan disimpan di folder `results/logs/`.

4. **Evaluasi Model**:
   - Setelah pelatihan selesai, model akan dievaluasi pada data pengujian dan menghasilkan metrik evaluasi seperti **accuracy**, **precision**, **recall**, **F1-score**, dan **AUC**.
   - Hasil evaluasi dan visualisasi akan disimpan di folder `results/visualizations/`.

5. **Model Terbaik**:
   - Model yang memiliki kinerja terbaik akan disimpan di folder `models/checkpoints/` untuk digunakan kembali di masa depan.

## Hasil Evaluasi

Berikut adalah hasil evaluasi model pada data pengujian:

```
Akurasi: 0.7500
Precision: 0.7899
Recall: 0.7365
F1-Score: 0.7499
AUC: 0.9152
```

**Laporan Klasifikasi**:
- **Basal Cell Carcinoma**: Precision = 0.7917, Recall = 0.7755, F1-Score = 0.7835
- **Melanoma**: Precision = 0.7091, Recall = 0.7800, F1-Score = 0.7429
- **Keratosis Aktinik**: Precision = 0.7556, Recall = 0.6939, F1-Score = 0.7234

## Referensi

- **Transfer Learning for Image Classification** - [Link ke artikel referensi]
- **VGGNet: Visual Geometry Group Network** - [Link ke artikel referensi]
- **MobileNet: Lightweight Deep Learning** - [Link ke artikel referensi]

## Kontribusi

Jika Anda ingin berkontribusi pada proyek ini, silakan fork repositori ini dan kirimkan pull request. Semua kontribusi yang relevan dan membantu untuk memperbaiki atau mengembangkan model ini akan diterima dengan senang hati.

## Lisensi

Proyek ini dilisensikan di bawah **MIT License** - lihat file [LICENSE](LICENSE) untuk detail lebih lanjut.

## Kontak

Jika Anda memiliki pertanyaan atau ingin berdiskusi lebih lanjut tentang proyek ini, silakan hubungi saya di:
- **Email**: example@example.com
- **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/example)
