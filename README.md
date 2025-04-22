# Certainty Factor & Fuzzy Logic
## 🔹 Certainty Factor (CF)
Certainty Factor adalah metode dalam sistem pakar yang digunakan untuk menangani ketidakpastian dalam penalaran. Konsep ini berasal dari sistem MYCIN dan digunakan untuk mengukur tingkat keyakinan terhadap suatu fakta atau kesimpulan berdasarkan:

CF Pakar: Nilai kepercayaan dari seorang ahli terhadap hubungan antara gejala dan penyakit.

CF User: Nilai kepercayaan dari pengguna terhadap gejala yang dirasakan.

CF Gabungan dihitung dengan rumus kombinasi:
```
CF_total = CF1 + CF2 * (1 - CF1)
untuk penggabungan lebih dari satu gejala.
```
### ✅ Kelebihan:
Cocok untuk sistem pakar berbasis aturan.

Bisa menangani ketidakpastian dari berbagai sumber.

### 📌 Contoh:
Jika user merasakan gejala demam dengan CF 0.7 dan pakar memberikan CF 0.8 terhadap demam → flu, maka kontribusi gejala ini:
```
CF(demam) = 0.7 × 0.8 = 0.56
```
## 🔹 Fuzzy Logic
Fuzzy Logic adalah pendekatan logika yang menangani ketidakpastian nilai numerik dan memungkinkan input untuk memiliki derajat keanggotaan ganda.

Komponen Utama:
Variabel Linguistik: Misalnya 
```
temperature = dingin | nyaman | panas.
```
Fungsi Keanggotaan (Membership Function): Menentukan tingkat keanggotaan nilai numerik ke dalam kategori linguistik (misalnya menggunakan trimf, trapmf).

Aturan IF-THEN (Fuzzy Rules): Contoh:
```
Jika suhu panas dan kelembaban lembab → kecepatan kipas = maksimal
```
Inferensi Fuzzy: Menentukan output berdasarkan aturan dan derajat keanggotaan input.

Defuzzifikasi: Mengubah hasil fuzzy ke bentuk numerik yang bisa digunakan, seperti fan_speed = 83%.

### ✅ Kelebihan:
Meniru cara berpikir manusia dalam mengambil keputusan.

Cocok untuk pengendalian sistem fisik, seperti AC, mesin cuci, mobil pintar, dll.

### 📌 Contoh:
Jika suhu 28°C, maka suhu dapat tergolong:
```
nyaman dengan derajat 0.4
panas dengan derajat 0.6
```
Keduanya diproses dalam aturan fuzzy untuk menentukan output akhir.

