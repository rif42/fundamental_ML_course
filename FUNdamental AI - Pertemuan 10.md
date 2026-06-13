---
width: "1920"
---
# Pertemuan 10

# Neural Network dan Deep Learning

---

![[Pasted image 20251124132205.png]]

---

Di pertemuan 9, kita belajar tentang artificial neuron dan natural neuron

Apa yang di olah oleh natural neuron? <!-- element class="fragment"   -->

### impuls atau sinyal elektrik <!-- element class="fragment"   -->

Apa yang di olah oleh artificial neuron? <!-- element class="fragment"-->

### angka <!-- element class="fragment"   -->


---

## Neural Network

neural adalah **sesuatu yang terdiri dari sel neuron** <!-- element class="fragment"   -->

network adalah **jaringan atau sistem koneksi** <!-- element class="fragment"   -->

sekarang, kita akan mempelajari tentang bagaimana neuron membentuk sebuah jaringan <!-- element class="fragment"   -->

---

### Komponen

Neural Network terdiri dari 3 bagian

- input layer (merah)
- hidden layer (biru)
- output layer (hijau)

![[Pasted image 20251124104944.png]]

---

<strong>Input Layer</strong> adalah panca indera dari neural network. Tempat dimana data masuk dan diterima. Data ini bisa berbentuk gambar, suara, atau teks yang dikonversi menjadi angka sebelum masuk ke input layer <!-- element class="fragment"   -->

<strong>Hidden Layer</strong> adalah bagian internal yang berfungsi memproses informasi dengan mencari pola atau pattern dari sebuah data. Lapisan ini dinamakan "Hidden" karena nilai-nilai yang ada di dalam hidden layer tidak tampak ke user, hanya output nya saja <!-- element class="fragment"   -->

<strong>Output Layer</strong> adalah hasil dari proses kalkulasi yang terjadi di neural network. Hasil ini dapat berupa prediksi atau klasifikasi yang data nya berbentuk angka. <!-- element class="fragment"   -->

---

### Analogi

<split even >

![[Pasted image 20251124134121.png]]

<br><br>(Ingat, ini adalah versi simpel nya)  <br><br>
musik yang bermain adalah **input**<br><br>
masing-masing knob adalah volume yang mengatur seberapa keras suara instrumen. knob adalah **weight**  <br><br>
hasilnya, ada 2, musik yang harmonis, atau suara random yang tidak enak didengar. musik adalah **output** <br><br>
ketika program ini dijalankan, knob volume akan teracak.  <br><br>
tugas anda adalah menemukan kombinasi knob volume yang pas agar bisa menghasilkan sebuah musik yang enak didengar 
</split>

---
## Versi Real
<iframe width="760" height="515" src="https://www.youtube.com/embed/aircAruvnKk?si=x_NcTP7zH6ajIsxo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Apa itu Deep Learning?

![[Pasted image 20251124142609.png]]<!-- element class="fragment"   -->


---


Deep learning adalah neural network yang terdiri dari lebih dari 3 hidden layers.

Mengapa harus 3 layer?<!-- element class="fragment"   -->

Hidden layer ini mengandung fitur-fitur "mentah" yang di ekstrak dari data.<!-- element class="fragment"   -->

Neural network biasa hanya bisa mendeteksi fitur atau pola dari data secara "surface level"<!-- element class="fragment"   -->

ketika layer diperbanyak, neural network bisa mempelajari fitur atau pola yang jauh lebih kompleks<!-- element class="fragment"   -->

---

## Jenis-Jenis Deep Learning

Deep Learning mempunyai aplikasi yang sangat amat luas

Tujuan utama dari deep learning adalah meng-ekstrak pola atau makna dari data <!-- element class="fragment"   -->

Tidak semua bentuk data sama, ada yang terdiri dari biner (angka 1 dan 0), ada yang terdiri dari pecahan. <!-- element class="fragment"   -->

Pola dari data pun juga berbeda-beda <!-- element class="fragment"   -->

Oleh karena itu, kita harus menggunakan jenis deep learning yang tepat untuk bentuk data dan jenis pola yang tepat. <!-- element class="fragment"   -->

---

### Convolutional Neural Network (CNN)

CNN biasanya digunakan untuk mengolah gambar

gambar mempunyai bentuk data 2 dimensi (tabel)<!-- element class="fragment"   -->

ketika kita mendapatkan "makna" dari sebuah gambar, maka kita bisa mendeteksi objek yang ada di dalam gambar tersebut (object detection) <!-- element class="fragment"   -->

---


https://youtu.be/aircAruvnKk?si=kLWWz1bgE_R-crsJ&t=413


---

### Contoh Object Detection di dunia nyata :

#### Anjing atau Cookies? <!-- element class="fragment"   -->

![[Pasted image 20251124145328.png]]<!-- element class="fragment"   -->

---

### Recurrent Neural Network (RNN)

RNN biasanya digunakan untuk mengambil makna dari data yang berbentuk sequential, atau berurutan.

tujuannya adalah menggunakan makna yang didapatkan untuk memprediksi kata yang muncul setelahnya, mirip seperti fitur predictive text di autocorrect  <!-- element class="fragment"   -->

data sequential berarti jika urutan diganti, maka arti ikut berubah <!-- element class="fragment"   -->

contohnya?  bahasa yang kita gunakan sehari hari <!-- element class="fragment"   -->

---

#### "Aku makan ayam"

![[Pasted image 20251124150412.png]]<!-- element class="fragment"   -->

---

#### "Ayam makan aku"

![[Pasted image 20251124150438.png]]<!-- element class="fragment"   -->

---

Contoh1:

![[Pasted image 20251124152304.png]]

1. input awal di prediksi, hasil output "so"<!-- element class="fragment"   -->
2. lalu "so" (hasil output step 1) menjadi input di step 2, output nya "long"<!-- element class="fragment"   -->
3. "long" (hasil output step 2), menjadi input di step 3, output nya...<!-- element class="fragment"   -->


---

Contoh 2 - Long Short Term Memory (LSTM) :

![[Pasted image 20251124151917.png]]

LSTM adalah bentuk upgrade dari RNN <!-- element class="fragment"   -->

RNN hanya melihat satu kata kebelakang, tapi LSTM bisa melihat beberapa kata kebelakang, memperbesar "context window" nya.<!-- element class="fragment"   -->


---

### Transformer

Masih ingat dengan paper ini?

![[Pasted image 20251210094853.png|750]]

---
Paper ini menjelaskan tentang arsitektur deep learning baru

arsitektur ini tidak menggunakan sistem recurrent atau convolutional, tapi menggunakan attention <!-- element class="fragment"   -->

apa itu attention? <!-- element class="fragment"   -->

---
#### Study Case

![[Pasted image 20251210100148.png|500]]

ada berapa kata "MOLE" di kalimat kalimat diatas?

apa arti kata "MOLE" di masing masing kalimat?<!-- element class="fragment"   -->

---


![[Pasted image 20251210100251.png|500]]

kenapa bisa beda????? <!-- element class="fragment"   -->

---

konteks dari kata "mole" terletak di kata-kata sekitarnya

bisa di depan, bisa di belakang <!-- element class="fragment"   -->

bisa dekat, bisa jauh <!-- element class="fragment"   -->

apakah LSTM bisa "melihat" kebelakang lebih dari 4 kata? <!-- element class="fragment"   -->

inilah kelemahan utama dari LSTM <!-- element class="fragment"   -->

Transformer berfungsi untuk mengatasi kelemahan ini <!-- element class="fragment"   -->

---

kita akan mengaplikasikan mekanisme transformer ke sebuah kalimat yang kita ingin pahami.

kalimat tersebut adalah:

#### a fluffy blue creature roamed the verdant forest<!-- element class="fragment"   -->

---

#### Step 1

langkah pertama adalah untuk memecah kalimat menjadi token.

Token adalah satuan terkecil dari sebuah data teks yang mewakili sebuah makna, yang dapat dicerna oleh sistem komputer <!-- element class="fragment"   -->

![[Pasted image 20251210102158.png]] <!-- element class="fragment"   -->

---

#### Step 2

langkah kedua, adalah menentukan makna dari masing-masing kata, di dalam vakum.

di machine learning, MAKNA dan POSISI dari kata disimpan di dalam sebuah matriks vektor <!-- element class="fragment"   -->

![[Pasted image 20251210102555.png]]<!-- element class="fragment"   -->

---

kita juga bisa menggunakan gambar untuk mendeskripsikan makna

![[Pasted image 20251210102623.png]]

---


kita gunakan notasi E untuk menyimpan makna dari masing masing kata

![[Pasted image 20251210110458.png]]


---

#### Step 4

masing masing kata akan mengecek kata lainnya, dan bertanya "apakah kamu ada hubungannya denganku?"

![[Pasted image 20251210111028.png]]

---

#### Step 5

jika ada kata yang mempunyai relasi yang kuat, maka bisa dikatakan bahwa kata-kata tersebut berpasangan dan dapat mengubah arti dari kata awal.

![[Pasted image 20251210111227.png]]

---

menggunakan grafik lain, kita bisa lihat korelasi antara "creature" ke "blue" dan "fluffy".

korelasi nya sangat besar

![[Pasted image 20251210112330.png]]

---

ketika kalimat input diperpanjang, maka tabel juga membesar secara eksponensial

![[Pasted image 20251210112500.png]]

---

jadi, makna yang diambil dari kalimat 
#### a fluffy blue creature roamed the verdant forest

dapat di visualisasikan menjadi:

![[Gemini_Generated_Image_5xkwo65xkwo65xkw.png]]


---

Contoh lain:

apa arti kata "BANK"?

![[Pasted image 20251210113358.png]]

---

kata apa yang paling berpengaruh terhadap "BANK"? 

![[Pasted image 20251210113713.png]] <!-- element class="fragment"   -->

---

berarti arti dari "BANK" adalah.....

![[Pasted image 20251210113757.png]]<!-- element class="fragment"   -->

---

bagaimana dengan kata ini

![[Pasted image 20251210113827.png]]

---

![[Pasted image 20251210113844.png]]

---

![[Pasted image 20251210113904.png]]

---

# Kesimpulan

- neural network adalah sekumpulan neuron yang membentuk sebuah jaringan yang dapat memproses input menjadi output
- neural network mempunyai input layer, hidden layer, dan output layer <!-- element class="fragment"   -->
- deep learning adalah neural network yang mempunyai lebih dari 3 hidden layer <!-- element class="fragment"   -->
- fungsi dari hidden layer adalah untuk meng-ekstrak fitur-fitur dari sebuah input, lalu merekonstruksikannya menjadi sebuah output  <!-- element class="fragment"   -->
- tingkat keberhasilan atau akurasi dari deep learning model tergantung pada arsitektur deep learning, fitur yang dipelajari, dan bentuk data <!-- element class="fragment"   -->
- Convolutional Neural Network (CNN) digunakan untuk memproses gambar <!-- element class="fragment"   -->
- Recurrent Neural Network (RNN) digunakan untuk memproses data sequential (teks atau grafik berjenjang) <!-- element class="fragment"   -->
- Long Short-Term Memory (LSTM) adalah versi upgrade dari RNN  <!-- element class="fragment"   -->
- Transformer adalah versi upgrade dari LSTM, yang digunakan di hampir semua model modern <!-- element class="fragment"   -->
- Transformer bekerja dengan cara memetakan relasi antar kata dan mengambil makna kata dari relasi tersebut <!-- element class="fragment"   -->