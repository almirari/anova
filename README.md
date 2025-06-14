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

#### Rumus-Rumus

1. **Jumlah Kuadrat Total (SST - Total Sum of Squares)**

   ```
   SST = Σ(xij - x̄..)²
   ```

   Dimana:

   - xij = nilai observasi ke-j dalam kelompok ke-i
   - x̄.. = rata-rata keseluruhan (grand mean)

2. **Jumlah Kuadrat Antar Kelompok (SSB - Between Groups Sum of Squares)**

   ```
   SSB = Σni(x̄i. - x̄..)²
   ```

   Dimana:

   - ni = jumlah observasi dalam kelompok ke-i
   - x̄i. = rata-rata kelompok ke-i
   - x̄.. = rata-rata keseluruhan

3. **Jumlah Kuadrat Dalam Kelompok (SSW - Within Groups Sum of Squares)**

   ```
   SSW = ΣΣ(xij - x̄i.)²
   ```

   Dimana:

   - xij = nilai observasi ke-j dalam kelompok ke-i
   - x̄i. = rata-rata kelompok ke-i

4. **Statistik F**
   ```
   F = (SSB/(k-1)) / (SSW/(N-k))
   ```
   Dimana:
   - k = jumlah kelompok
   - N = total jumlah observasi
   - Derajat kebebasan (df) untuk pembilang = k-1
   - Derajat kebebasan (df) untuk penyebut = N-k

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

#### Rumus-Rumus ANOVA Dua Arah

1. **Jumlah Kuadrat Total (SST)**

   ```
   SST = ΣΣΣ(xijk - x̄...)²
   ```

   Dimana:

   - xijk = nilai observasi ke-k dalam kombinasi faktor i dan j
   - x̄... = rata-rata keseluruhan

2. **Jumlah Kuadrat Faktor A (SSA)**

   ```
   SSA = bnΣ(x̄i.. - x̄...)²
   ```

   Dimana:

   - b = jumlah level faktor B
   - n = jumlah replikasi
   - x̄i.. = rata-rata level ke-i faktor A
   - x̄... = rata-rata keseluruhan

3. **Jumlah Kuadrat Faktor B (SSB)**

   ```
   SSB = anΣ(x̄.j. - x̄...)²
   ```

   Dimana:

   - a = jumlah level faktor A
   - n = jumlah replikasi
   - x̄.j. = rata-rata level ke-j faktor B
   - x̄... = rata-rata keseluruhan

4. **Jumlah Kuadrat Interaksi (SSAB)**

   ```
   SSAB = nΣΣ(x̄ij. - x̄i.. - x̄.j. + x̄...)²
   ```

   Dimana:

   - x̄ij. = rata-rata kombinasi level i faktor A dan level j faktor B
   - x̄i.. = rata-rata level ke-i faktor A
   - x̄.j. = rata-rata level ke-j faktor B
   - x̄... = rata-rata keseluruhan

5. **Jumlah Kuadrat Error (SSE)**

   ```
   SSE = ΣΣΣ(xijk - x̄ij.)²
   ```

   Dimana:

   - xijk = nilai observasi ke-k dalam kombinasi faktor i dan j
   - x̄ij. = rata-rata kombinasi level i faktor A dan level j faktor B

6. **Statistik F untuk Setiap Efek**
   ```
   FA = (SSA/(a-1)) / (SSE/(ab(n-1)))
   FB = (SSB/(b-1)) / (SSE/(ab(n-1)))
   FAB = (SSAB/((a-1)(b-1))) / (SSE/(ab(n-1)))
   ```
   Dimana:
   - a = jumlah level faktor A
   - b = jumlah level faktor B
   - n = jumlah replikasi
   - Derajat kebebasan untuk pembilang FA = a-1
   - Derajat kebebasan untuk pembilang FB = b-1
   - Derajat kebebasan untuk pembilang FAB = (a-1)(b-1)
   - Derajat kebebasan untuk penyebut = ab(n-1)

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

### Tabel ANOVA

1. **ANOVA Satu Arah**
   | Sumber Variasi | Jumlah Kuadrat | Derajat Kebebasan | Rata-rata Kuadrat | F-statistik |
   |---------------|----------------|-------------------|-------------------|-------------|
   | Antar Kelompok | SSB | k-1 | MSB = SSB/(k-1) | F = MSB/MSE |
   | Dalam Kelompok | SSW | N-k | MSE = SSW/(N-k) | |
   | Total | SST | N-1 | | |

2. **ANOVA Dua Arah**
   | Sumber Variasi | Jumlah Kuadrat | Derajat Kebebasan | Rata-rata Kuadrat | F-statistik |
   |---------------|----------------|-------------------|-------------------|-------------|
   | Faktor A | SSA | a-1 | MSA = SSA/(a-1) | FA = MSA/MSE |
   | Faktor B | SSB | b-1 | MSB = SSB/(b-1) | FB = MSB/MSE |
   | Interaksi AB | SSAB | (a-1)(b-1) | MSAB = SSAB/((a-1)(b-1)) | FAB = MSAB/MSE |
   | Error | SSE | ab(n-1) | MSE = SSE/(ab(n-1)) | |
   | Total | SST | abn-1 | | |

Dimana:

- a = jumlah level faktor A
- b = jumlah level faktor B
- n = jumlah replikasi
- N = total jumlah observasi
- k = jumlah kelompok (untuk ANOVA satu arah)

### Implementasi

Repositori ini berisi implementasi analisis ANOVA Satu Arah dan Dua Arah menggunakan Python, dilengkapi dengan contoh detail dan visualisasi untuk membantu memahami hasil analisis.
