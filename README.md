# made7120-PREDIKSI-HARGA-SAHAM-TESLA-MENGGUNAKAN-MODEL-RECCURENT-NEURAL-NETWORK-RRN-LSTM-DAN-ARIMA
# Prediksi Harga Saham Tesla

Proyek ini bertujuan untuk memprediksi harga saham masa depan Tesla menggunakan tiga model yang berbeda: ARIMA, RNN, dan LSTM. Data yang digunakan dalam proyek ini adalah harga saham historis Tesla, yang diambil dari Yahoo Finance. Model-model ini dilatih dan dievaluasi untuk meramalkan harga penutupan saham untuk 10 hari ke depan.

## Deskripsi

Proyek ini mencakup:

- **Pengumpulan Data**: Data saham diambil menggunakan pustaka `yfinance`.
- **Pranala Data**: Data dibersihkan dan dipersiapkan untuk analisis (mengatasi nilai yang hilang, normalisasi).
- **Pemodelan**: Tiga model digunakan untuk memprediksi harga saham:
  1. **ARIMA (AutoRegressive Integrated Moving Average)**: Model ramalan deret waktu klasik.
  2. **RNN (Recurrent Neural Network)**: Model pembelajaran mendalam yang cocok untuk prediksi urutan.
  3. **LSTM (Long Short-Term Memory)**: Jenis RNN khusus yang menangani ketergantungan jangka panjang.
- **Evaluasi**: Model-model ini dievaluasi menggunakan Root Mean Squared Error (RMSE) untuk membandingkan kinerja prediksi mereka.

## Persyaratan

Untuk menjalankan kode ini, Anda perlu menginstal pustaka berikut:

- `yfinance`: Untuk mengambil data saham dari Yahoo Finance.
- `pandas`: Untuk manipulasi dan analisis data.
- `numpy`: Untuk operasi numerik.
- `matplotlib`: Untuk memvisualisasikan data dan hasil.
- `scikit-learn`: Untuk pra-pemrosesan data dan metrik evaluasi.
- `statsmodels`: Untuk model ARIMA.
- `tensorflow`: Untuk membangun dan melatih model RNN dan LSTM.

Anda dapat menginstal dependensi dengan perintah berikut:

```bash
pip install yfinance pandas numpy matplotlib scikit-learn statsmodels tensorflow


Struktur File

    Tasla_Stock_Updated_V2.csv: Dataset yang berisi harga saham historis Tesla.

    stock_price_prediction.py: Skrip Python yang mengimplementasikan pra-pemrosesan data, pelatihan model, dan evaluasi.

Cara Menggunakan

    Unggah Dataset: Pertama, unggah file CSV harga saham Tesla ke direktori kerja.

    Jalankan Skrip: Skrip ini akan memuat dataset, melakukan pra-pemrosesan, dan melatih model (ARIMA, RNN, dan LSTM) pada data historis.

    Lihat Hasil: Skrip ini akan menghasilkan harga saham yang diprediksi untuk 10 hari ke depan dan memplot hasilnya.

Perintah Contoh untuk Menjalankan:

python stock_price_prediction.ipynb

Hasil

Kinerja model dievaluasi menggunakan RMSE:

    RMSE ARIMA: 16.83

    RMSE RNN: 238.39

    RMSE LSTM: 229.55

Hasil ini menunjukkan seberapa baik masing-masing model dalam memprediksi harga saham Tesla berdasarkan data historis.
Visualisasi

Proyek ini mencakup plot dari:

    Harga saham Tesla historis.

    Harga saham yang diprediksi menggunakan model ARIMA, RNN, dan LSTM.
