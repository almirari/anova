# Analisis Varians (ANOVA)

| Nama                                  | NRP        | Kelas                           |
| ------------------------------------- | ---------- | ------------------------------- |
| Ainun Nadhifah Syamsiyah              | 5025221053 | Probabilitas dan Statistika (A) |
| Richard Halomoan Sitanggang           | 5025221117 | Probabilitas dan Statistika (A) |
| Willyam Brordus Dominikus Simanihuruk | 5025221121 | Probabilitas dan Statistika (A) |
| Almira Raisa Izzatina                 | 5025221250 | Probabilitas dan Statistika (A) |

## Analisis Varians (ANOVA)

Analisis Varians (ANOVA) adalah metode statistik yang digunakan untuk menguji perbedaan antara dua atau lebih rata-rata. Metode ini membantu menentukan apakah perbedaan antar kelompok signifikan secara statistik atau hanya terjadi secara kebetulan.

### ANOVA Satu Arah (One-Way ANOVA)

ANOVA satu arah digunakan ketika kita ingin membandingkan rata-rata dari tiga atau lebih kelompok berdasarkan satu variabel independen (faktor).

#### Karakteristik Utama:

- Satu variabel independen (faktor)
- Tiga atau lebih kelompok/tingkat
- Satu variabel dependen
- Menguji hipotesis nol bahwa semua rata-rata kelompok sama

#### Contoh Penggunaan:

- Membandingkan nilai ujian dari berbagai metode pengajaran
- Menganalisis pengaruh berbagai jenis pupuk terhadap pertumbuhan tanaman
- Mengevaluasi dampak berbagai jenis diet terhadap penurunan berat badan

#### Asumsi:

1. Independensi observasi
2. Distribusi normal dari residual
3. Homogenitas varians (varians sama antar kelompok)

### ANOVA Dua Arah (Two-Way ANOVA)

ANOVA dua arah digunakan ketika kita ingin menganalisis pengaruh dua variabel independen (faktor) terhadap variabel dependen, dan juga memeriksa apakah ada efek interaksi antara kedua faktor tersebut.

#### Karakteristik Utama:

- Dua variabel independen (faktor)
- Beberapa kelompok/tingkat untuk setiap faktor
- Satu variabel dependen
- Menguji tiga hipotesis:
  - Efek utama faktor pertama
  - Efek utama faktor kedua
  - Efek interaksi antar faktor

#### Contoh Penggunaan:

- Mempelajari pengaruh jenis kelamin dan jenis olahraga terhadap penurunan berat badan
- Menganalisis bagaimana suhu dan kelembaban mempengaruhi pertumbuhan tanaman
- Mengevaluasi dampak metode pengajaran dan ukuran kelas terhadap performa siswa

#### Asumsi:

1. Independensi observasi
2. Distribusi normal dari residual
3. Homogenitas varians
4. Tidak ada pencilan (outlier) yang signifikan

### Kapan Menggunakan Masing-masing Jenis

- Gunakan **ANOVA Satu Arah** ketika:

  - Anda memiliki satu variabel independen
  - Anda ingin membandingkan rata-rata dari tiga atau lebih kelompok
  - Anda tertarik pada efek dari satu faktor

- Gunakan **ANOVA Dua Arah** ketika:
  - Anda memiliki dua variabel independen
  - Anda ingin menganalisis efek dari masing-masing faktor
  - Anda ingin memeriksa apakah ada interaksi antar faktor
  - Anda perlu memahami bagaimana dua faktor bekerja bersama

### Interpretasi Hasil

#### ANOVA Satu Arah:

- Statistik-F: Menunjukkan apakah ada perbedaan signifikan antar rata-rata kelompok
- Nilai-p: Menentukan signifikansi statistik (biasanya < 0,05)
- Uji post-hoc: Mengidentifikasi kelompok mana yang berbeda satu sama lain

#### ANOVA Dua Arah:

- Statistik-F: Tiga uji-F (satu untuk setiap efek utama dan satu untuk interaksi)
- Nilai-p: Untuk setiap efek
- Plot interaksi: Memvisualisasikan bagaimana faktor-faktor berinteraksi
- Efek utama: Dampak individual dari setiap faktor
- Efek interaksi: Bagaimana faktor-faktor bekerja bersama

### Implementasi

Repositori ini berisi implementasi analisis ANOVA Satu Arah dan Dua Arah menggunakan Python, dilengkapi dengan contoh detail dan visualisasi untuk membantu memahami hasil analisis.
