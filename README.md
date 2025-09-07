# Analisis Sentimen Media Sosial dan Dampaknya terhadap Harga Bitcoin (Studi Kasus: 2023)

## Project Overview
Harga mata uang kripto seperti Bitcoin dikenal sangat volatil dan dipengaruhi oleh banyak faktor. Salah satu faktor kunci yang diduga memiliki pengaruh kuat adalah sentimen publik yang tecermin dalam diskusi di media sosial. Investor dan analis sering kali kesulitan mengukur sentimen ini secara objektif dan memahami hubungannya dengan pergerakan pasar. Proyek ini bertujuan untuk menjembatani kesenjangan tersebut dengan menganalisis secara kuantitatif hubungan antara sentimen publik di platform media sosial dengan data historis harga Bitcoin.

## Google Colab Notebook
Berikut merupakan hasil proyek menggunakan google colab : 
Link: [[Link Colab](https://colab.research.google.com/drive/1FoxjJXftx9rSZnNokrFBBSGno9_yi8es?usp=sharing)]

## Raw Dataset Link
Proyek ini menggunakan dua dataset publik yang bersumber dari Kaggle.
- Dataset Harga Bitcoin Historis (2018-2023): Berisi data harga per jam (Open, High, Low, Close, Volume).
  Link: [[Link Dataset](https://www.kaggle.com/datasets/novandraanugrah/bitcoin-historical-datasets-2018-2024)]
    
- Dataset Tweet Bitcoin: Berisi kumpulan tweet mengenai Bitcoin.
  Link: [[Link Dataset](https://www.kaggle.com/datasets/kaushiksuresh147/bitcoin-tweets/data)]

## Insight & Findings
Setelah melalui proses pembersihan, penggabungan, dan analisis data, berikut adalah temuan-temuan utama dari proyek ini:
- Stabilitas Sentimen Publik: Temuan yang paling signifikan adalah bahwa sentimen rata-rata harian publik terhadap Bitcoin cenderung stabil dan netral sepanjang tahun 2023. Analisis distribusi menunjukkan bahwa mayoritas besar (lebih dari 80%) tweet diklasifikasikan sebagai "Netral".
- Sentimen Bukan Indikator Utama: Akibat dari rendahnya variasi pada data sentimen, grafik sentimen harian menunjukkan garis yang relatif datar. Hal ini mengindikasikan bahwa rata-rata sentimen harian bukan merupakan indikator yang kuat atau reliable untuk memprediksi pergerakan harga Bitcoin dalam jangka pendek.
- Diskusi Sosial Bersifat Reaktif, Bukan Prediktif: Momen puncak diskusi sosial (volume tweet) tidak selalu bertepatan langsung dengan lonjakan harga. Seringkali, lonjakan diskusi terjadi setelah pergerakan harga yang signifikan. Ini menunjukkan bahwa percakapan di media sosial lebih bersifat reaktif terhadap kondisi pasar daripada menjadi pemicu utamanya.

## AI Support Explanation
Penggunaan model AI, khususnya IBM Granite melalui API, memegang peranan krusial dalam dua tahap utama proyek ini:
    Klasifikasi Sentimen Skala Besar: Dataset sentimen berisi puluhan ribu tweet dalam bentuk teks mentah. Mengklasifikasikannya secara manual menjadi "Positif", "Negatif", atau "Netral" tidaklah mungkin. IBM Granite digunakan untuk mengotomatiskan proses ini. Sebuah fungsi Python dibuat untuk mengirim setiap teks tweet ke model dan menerima kembali label sentimennya. Hal ini memungkinkan pemrosesan data tekstual dalam jumlah besar secara cepat dan konsisten.
    
    Gambar terlampir mengenai beberapa screenshot hasil penggunaan IBM-Granite pada lampiran file.
