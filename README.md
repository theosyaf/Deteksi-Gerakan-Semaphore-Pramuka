# Real-Time Semaphore Detection System 🚩

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/framework-TensorFlow-orange.svg)](https://www.tensorflow.org/)

## 📝 Deskripsi Proyek

Penelitian ini bertujuan untuk mendigitalkan penerjemahan sandi Semaphore pramuka menggunakan pendekatan *Deep Learning*. Tantangan utama dalam deteksi gerakan tubuh secara *real-time* 
adalah tingginya biaya komputasi jika menggunakan pemrosesan citra langsung (2D CNN).

Sebagai solusi, proyek ini mengusulkan pendekatan hibrida:
1.  **Ekstraksi Fitur:** Menggunakan **MediaPipe Pose** untuk mendeteksi *landmark* tubuh dan mengonversinya menjadi koordinat vektor.
2.  **Klasifikasi:** Menggunakan arsitektur **1D Convolutional Neural Network (CNN)** untuk memproses data vektor tersebut.

Metode ini memungkinkan sistem berjalan dengan latensi rendah pada perangkat dengan spesifikasi terbatas, tanpa mengorbankan akurasi secara signifikan.

## 🚀 Fitur Utama

* **Real-time Detection:** Menerjemahkan gerakan tangan menjadi huruf abjad secara langsung lewat webcam.
* **Lightweight Architecture:** Menggunakan input data 1D (koordinat x, y, z, visibility) yang jauh lebih ringan dibanding input piksel gambar.
* **Model Comparison:** Menyediakan implementasi dan perbandingan performa (akurasi & loss) dari tiga arsitektur:
    * LeNet-5 (Modified for 1D)
    * VGG-Like Network
    * ResNet-Like Network

## 🛠️ Teknologi yang Digunakan

* **Bahasa:** Python
* **Computer Vision:** OpenCV, MediaPipe
* **Deep Learning:** TensorFlow / Keras
* **Data Handling:** NumPy

## 📊 Hasil Penelitian

*Ringkasan singkat hasil :*
* Model **LeNet-5** mencapai akurasi tertinggi sebesar **70.626**.
* Jumlah Parameter adalah **XX ms**.

---
*Proyek ini merupakan bagian dari Skripsi S1 Teknik Informatika, Fakultas Teknik, Universitas Hasanuddin.*
