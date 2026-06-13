---
width: "1920"
---
# Pertemuan 11

# Machine Learning dan Proses Training

---

![[Pasted image 20251124132205.png]]

---
# Definisi

Tujuan utama dari model machine learning adalah untuk melakukan sesuatu tanpa harus di program

untuk melakukannya, model machine learning harus memproses data, belajar dari data, dan berkembang untuk melakukan sesuatu secara akurat <!-- element class="fragment"   -->

---

#### secara garis besar, proses pembuatan model mempunyai tahap-tahap:
- data processing<!-- element class="fragment"   -->
- pemilihan algoritma<!-- element class="fragment"   -->
- proses training<!-- element class="fragment"   -->
- evaluasi<!-- element class="fragment"   -->

---
# Data Processing

Data adalah faktor terpenting di model machine learning

langkah pertama adalah untuk menemukan atau mencari data<!-- element class="fragment"   -->

langkah kedua, membersihkan data (dari nilai kosong, invalid, dll) <!-- element class="fragment"   -->

langkah ketiga, memahami data, fitur apa yang penting/tidak penting, hubungan antar fitur, bentuk data, jumlah data <!-- element class="fragment"   -->

sebagai seorang machine learning engineer, sebagian besar waktu kalian akan digunakan untuk langkah kedua  <!-- element class="fragment"   -->

---
# Data Processing

langkah keempat, besar kemungkinan bahwa data harus diolah terlebih dahulu sebelum masuk ke machine learning model 

maka kita harus melakukan grouping, penggabungan fitur, penyederhanaan fitur, dll. inilah namanya feature engineering <!-- element class="fragment"   --> 

fitur ini adalah INTI dari skill seorang machine learning engineer. <!-- element class="fragment"   -->

setelah itu, kita bisa menentukan algoritma apa yang kita pilih untuk proses training <!-- element class="fragment"   -->

---

# Jenis Machine Learning Model

## Hubungan Antar Fitur - Linear

semakin besar X, maka semakin besar Y (garis lurus)

Jika 5 tukang bisa membangun sebuah rumah dalam 2 minggu, maka berapa tukang yang dibutuhkan untuk membangun rumah dalam 3 hari?

---

contoh lain: 

![[Pasted image 20251210141247.png]]

---

![[Pasted image 20251210141420.png]]

---

## Hubungan Antar Fitur - Non Linear

semakin besar X, semakin besar Y. Tapi jika X melebihi Z, maka Y mengecil (garis kurva / bengkok)

jika 2 handuk basah dijemur di dapat kering dalam 2 jam, maka berapa waktu yang dibutuhkan untuk mengeringkan 8 handuk basah? asumsikan bahwa matahari tetap bersinar sepanjang waktu

---
contoh  :

![[Pasted image 20251210141225.png]]


---
## Jenis Pekerjaan - Regresi / Prediksi

sebuah teknik statistik yang berguna untuk menemukan relasi antara variabel/fitur dan label.

regresi MEMBUTUHKAN LABEL DATA

sebagai contoh, kita punya tabel dibawah ini 

| Pounds in 1000s (feature) | Miles per gallon (label) |
| ------------------------- | ------------------------ |
| 3.5                       | 18                       |
| 3.69                      | 15                       |
| 3.44                      | 18                       |
| 3.43                      | 16                       |
| 4.34                      | 15                       |
| 4.42                      | 14                       |
| 2.37                      | 24                       |

---

kita bisa ubah tabel tersebut menjadi grafik / plot

![[Pasted image 20251210131235.png]]

kira kira apa hubungan antar fiturnya apa?<!-- element class="fragment"   -->

---

hubungan antar fitur adalah LINEAR, maka kita bisa menggunakan algoritma LINEAR REGRESSION.

yang dilakukan linear regression adalah memprediksi hasil dari pertanyaan ini:<!-- element class="fragment"   -->

"jika berat dari mobil adalah 3000 pound, maka berapa mpg yang dipunyai mobil tersebut?"<!-- element class="fragment"   -->

![[Pasted image 20251210131406.png]]<!-- element class="fragment"   -->

---

## Jenis Pekerjaan - Klustering 

sebuah teknik statistik yang berfungsi untuk mengorganisir data menjadi grup-grup/klasifikasi tertentu berdasarkan tingkat kesamaan fitur.

klustering TIDAK MEMBUTUHKAN LABEL DATA

bentuk data linear (sama seperti sebelumnya)

| Pounds in 1000s (feature) | Miles per gallon (label) | Klasifikasi |
| ------------------------- | ------------------------ | ----------- |
| 3.5                       | 18                       | X           |
| 3.69                      | 15                       | X           |
| 3.44                      | 18                       | X           |
| 3.43                      | 16                       | X           |
| 4.34                      | 15                       | X           |
| 4.42                      | 14                       | X           |
| 2.37                      | 24                       | X           |

---

kita bisa menggunakan K-MEANS untuk menentukan klasifikasi dari kedua data.

Algoritma K-MEANS menghitung jarak antara poin-poin data. <!-- element class="fragment"   -->

jika jarak antara data 1 dan data 2 dekat, maka besar kemungkinan, kedua data tersebut berada di satu klasifikasi yang sama <!-- element class="fragment"   -->

Algoritma K-Means membutuhkan sebuah input, yaitu jumlah dari klasifikasi. nilai ini biasa disebut `k` <!-- element class="fragment"   -->

kira kira ada berapa jenis atau klasifikasi mobil berdasarkan data diatas? <!-- element class="fragment"   -->

---

jika `k` adalah 2, maka hasil dari clusterization adalah:

![[Pasted image 20251210144237.png]]

---
## Jenis Pekerjaan - Klasifikasi 

sebuah teknik statistik yang memprediksi klasifikasi dari sebuah data baru.

bentuk data linear (sama seperti sebelumnya)

klasifikasi MEMBUTUHKAN LABEL DATA

| Pounds in 1000s (feature) | Miles per gallon (label) | Klasifikasi |
| ------------------------- | ------------------------ | ----------- |
| 3.5                       | 18                       | truck       |
| 3.69                      | 15                       | truck       |
| 3.44                      | 18                       | truck       |
| 3.43                      | 16                       | X           |
| 4.34                      | 15                       | truck       |
| 4.42                      | 14                       | truck       |
| 2.37                      | 24                       | mobil       |

apa klasifikasi dari row X? truck atau mobil?

---

untuk pekerjaan KLASIFIKASI LINEAR, kita bisa menggunakan algoritma K-MEANS

Data X termasuk kategori "truck" karena letaknya yang berdekatan

![[Pasted image 20251210135747.png]]

---

| **Feature**       | **Regression**        | **Classification**    | **Clustering**                  |
| ----------------- | --------------------- | --------------------- | ------------------------------- |
| **Learning Type** | **Supervised**        | **Supervised**        | **Unsupervised**                |
| **Input**         | Labeled Data $(X, y)$ | Labeled Data $(X, y)$ | Unlabeled Data $(X)$            |
| **Output**        | Angka                 | Teks/Klasifikasi      | **Group ID**                    |
| **Tujuan**        | Memprediksi data      | Mengidentifikasi data | Menemukan pola data tersembunyi |

---

# Proses Training - Thought Experiment

---

### Lupakan semua ingatan anda tentang buah buahan dan hewan.


kita akan menjadi sebuah model machine learning yang sedang diajarkan training data. <!-- element class="fragment"   -->

saya beri waktu 10 detik<!-- element class="fragment"   -->

---

#### Ada yang tahu semangka warnanya apa? <!-- element class="fragment"   -->

#### Berapa jumlah kaki dari seekor ayam? <!-- element class="fragment"   -->

oke berarti anda siap untuk di training <!-- element class="fragment"   -->

---

#### Kita sedang PROSES TRAINING, lihatlah gambar ini

  ![[orange_istock_000001331357x_540x405.jpg|500]]
  
- warnanya apa? **oranye<!-- element class="fragment"   -->**
- bentuknya apa? **bulat<!-- element class="fragment"   -->**
- tekstur kulit seperti apa? **halus tapi tidak rata<!-- element class="fragment"   -->

---

![[orange_istock_000001331357x_540x405.jpg|500]]

warna, bentuk, tekstur adalah FITUR DATA

sekarang saya kasih tahu ke kalian, bahwa gambar ini adalah BUAH JERUK <!-- element class="fragment"   -->

karena sudah saya kasih tahu, berarti data MEMPUNYAI LABEL<!-- element class="fragment"   -->

---
![[orange_istock_000001331357x_540x405.jpg|500]]

dari fitur-fitur tersebut, kita bisa menarik KESIMPULAN, bahwa "jika sesuatu warnanya oranye, bentuknya bulat, dan teksturnya halus tapi tidak rata, maka itu adalah jeruk"

kesimpulan ini diambil dari proses analisa fitur dan pengetahuan label data. inilah yang dinamakan PATTERN RECOGNITION atau PEMBELAJARAN POLA <!-- element class="fragment"   -->

PROSES TRAINING SELESAI <!-- element class="fragment"   -->

---

#### Kita sedang PROSES PREDIKSI, lihatlah gambar dibawah ini

![[Pasted image 20251210151042.png]]

- warnanya apa? **oranye**<!-- element class="fragment"   -->
- bentuknya apa? **bulat<!-- element class="fragment"   -->**
- teksturnya seperti apa? **halus tapi tidak rata<!-- element class="fragment"   -->**

---

![[Pasted image 20251210151042.png]]
#### Apakah ini jeruk?

yakin?????? <!-- element class="fragment"-->

seberapa yakin? <!-- element class="fragment"-->

bisa dibilang bahwa gambar diatas adalah "20% yakin bahwa gambar diatas adalah jeruk". <!-- element class="fragment"-->

---

![[Pasted image 20251210151042.png]]

20% adalah CONFIDENCE LEVEL, seberapa yakin kita (Sebuah model) dengan prediksi kita. 20% bukanlah angka yang baik  <!-- element class="fragment"-->

jika tingkat confidence level kita 80%, belum tentu hasil itu benar (sesuai dengan ground truth/kenyataan). inilah yang dinamakan ACCURACY <!-- element class="fragment"--> 

umumnya, model yang "bagus" harus mempunyai akurasi diatas 90%. Jika untuk kepentingan medis, standar itu naik jadi 98% atau bahkan 99%. <!-- element class="fragment"-->


---
#### Selanjutnya, bagaimana cara kita menambah akurasi model?

- tambah jumlah dataset, jeruk dari angle lain, jeruk jenis lain, atau gambar zoom ke bagian-bagian jeruk.<!-- element class="fragment"-->
- tambah jumlah fitur, rasa jeruk seperti apa, beratnya berapa, diameter atau ukurannya berapa cm.<!-- element class="fragment"-->
- perluas dataset, jangan cuma belajar tentang jeruk, tapi buah buahan lain juga, mungkin perluas ke hewan, termasuk kucing.<!-- element class="fragment"-->
- train data nya lebih dari 1 kali, di contoh atas kita cuma pelajari gambar 1x, kita bisa melakukannya berkali2. hal ini disebut TRAINING EPOCH.<!-- element class="fragment"-->

---

secara klasifikasi, kita baru saja mentraining model OBJECT DETECTION (klasifikasi) dengan cara SUPERVISED, karena kita memberikan LABEL dalam dataset kita. 

karena kita menggunakan model klasifikasi, maka bagaimana cara kita mengevaluasi model?

---

# Evaluasi

untuk model klasifikasi, metode evaluasi yang digunakan adalah "AKURASI"

ketika model diberikan data yang belum pernah dilihat, seberapa sering model memprediksi data tersebut dengan benar?

contohnya model diatas tujuannya untuk membedakan bahwa gambar adalah jeruk atau bukan, jadi kita beri gambar semangka.

---

ketika kita beri gambar semangka, lalu model menjawab "ini bukan jeruk", inilah yang dinamakan TRUE NEGATIVE (TN)

ketika kita beri gambar semangka, tetapi model malah menjawab "ya, ini jeruk", inilah yang dinamakan FALSE POSITIVE (FP)


Confusion Matrix

|                    | actual positive | actual negative                                 |
| ------------------ | --------------- | ----------------------------------------------- |
| predicted positive |                 | aslinya semangka, model bilang jeruk (FP)       |
| predicted negative |                 | aslinya semangka, model bilang bukan jeruk (TN) |


---

ketika kita beri gambar jeruk, lalu model menjawab "ini bukan jeruk", inilah yang dinamakan FALSE NEGATIVE (FN)

ketika kita beri gambar jeruk, lalu model menjawab "ya, ini jeruk", inilah yang dinamakan TRUE POSITIVE (TP)

Confusion Matrix

|                    | actual positive                              | actual negative                                 |
| ------------------ | -------------------------------------------- | ----------------------------------------------- |
| predicted positive | aslinya jeruk, model bilang jeruk (TP)       | aslinya semangka, model bilang jeruk (FP)       |
| predicted negative | aslinya jeruk, model bilang bukan jeruk (FN) | aslinya semangka, model bilang bukan jeruk (TN) |

---

ketika kita sudah mendapatkan semua nilai, maka kita bisa hitung akurasi nya :

$$\text{Accuracy} = \frac{\text{True Positives (TP)} + \text{True Negatives (TN)}}{\text{Total Samples}}$$

---
