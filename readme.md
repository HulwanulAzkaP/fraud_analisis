# Deteksi Penipuan Transaksi Kartu Kredit

## Deskripsi Proyek
Proyek ini bertujuan untuk mengembangkan model deteksi penipuan menggunakan machine learning yang dapat mengidentifikasi transaksi kartu kredit yang mencurigakan. Dengan meningkatnya kasus penipuan, model ini diharapkan dapat membantu lembaga keuangan untuk mencegah kerugian dan melindungi pengguna.

## Tujuan Proyek
- Membangun model untuk mendeteksi transaksi fraudulent secara akurat.
- Mengurangi jumlah false negatives.
- Mengidentifikasi pola transaksi yang mencurigakan.

## Dataset
Dataset yang digunakan adalah kumpulan transaksi kartu kredit yang mencakup atribut sebagai berikut:
- **ID**: Identifier unik untuk setiap transaksi.
- **V1-V28**: 28 fitur yang berhubungan dengan transaksi.
- **Amount**: Nilai moneter dari transaksi.
- **Class**: Kategori transaksi (0 untuk legitimate, 1 untuk fraudulent).

## Metodologi
1. **Pengumpulan Data**: Dataset diperoleh dari sumber publik.
2. **Preprocessing Data**:
   - Memeriksa dan menangani nilai hilang.
   - Memastikan tipe data kolom sesuai.
3. **Pembagian Dataset**: Membagi data menjadi set latih (70%) dan set uji (30%).
4. **Penyusunan Fitur**: Menggunakan `VectorAssembler` untuk menyusun fitur.
5. **Pelatihan Model**: Menggunakan algoritma **Random Forest Classifier**.
6. **Evaluasi Model**: Mengukur akurasi, precision, recall, dan F1-score.

## Hasil
Model mencapai:
- **Akurasi**: 95%
- **Precision**: 99%
- **Recall**: 91%
- **F1 Score**: 95%

### Confusion Matrix
|                | Predicted: Legitimate | Predicted: Fraudulent |
|----------------|-----------------------|-----------------------|
| Actual: Legitimate | 84853                 | 401                   |
| Actual: Fraudulent | 7423                  | 77910                 |

### Distribusi Prediksi
Distribusi menunjukkan jumlah transaksi yang dikategorikan sebagai legitimate dan fraudulent.
