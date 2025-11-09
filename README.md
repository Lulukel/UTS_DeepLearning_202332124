# UTS_DeepLearning_202332124
# PERBANDINGAN MODEL CNN DARI NOL DAN TRANSFER LEARNING PADA KLASIFIKASI ANGKA
## Proyek Ujian Tengah Semester (UTS) Praktikum Deep Learning

### Disusun oleh: Lulu El Maknun
### NIM: 202332124

 1. Tujuan Proyek

Proyek ini bertujuan utama untuk menguji dan membandingkan dua pendekatan fundamental dalam klasifikasi citra pada dataset MNIST (Handwritten Digit Recognition):

1.  **Model A (CNN dari Nol):** Mengukur efektivitas arsitektur *Convolutional Neural Network* (CNN) sederhana yang dibangun *from scratch*.
2.  **Model B (Transfer Learning):** Mengukur kemampuan adaptasi model *pre-trained* VGG16 sebagai *feature extractor*.

Fokus utama pengujian adalah pada kemampuan generalisasi kedua model ketika dihadapkan pada **30 citra tulisan tangan pribadi** yang merepresentasikan digit **1, 2, dan 4** (sesuai tiga angka terakhir NIM).



 2. Struktur Repositori & Data

Repositori ini harus memiliki struktur file sebagai berikut agar *notebook* dapat berjalan tanpa *error* dan instruksi pengumpulan terpenuhi:

| File/Folder | Keterangan |
| :--- | :--- |
| `UTS_DEEPL_202332124.ipynb` | **File utama** berisi seluruh kode: Pra-pemrosesan, pelatihan Model A, pelatihan Model B, dan evaluasi perbandingan. |
| `README.md` | File instruksi ini. |
| `UTS_tulisan_tangan/` | **Folder Wajib.** Berisi 30 citra (.jpg atau .png) tulisan tangan pribadi (1, 2, 4) yang digunakan untuk pengujian *out-of-domain*. |

---

3. Prasyarat (Dependencies)

Kode proyek ini diimplementasikan menggunakan Python dan TensorFlow/Keras. *n menggunakan Google Colab* dengan akselerator **GPU/T4** untuk mempercepat proses pelatihan Model B (VGG16) yang intensif.

Pustaka yang dibutuhkan:

```bash
pip install tensorflow keras numpy matplotlib opencv-python
