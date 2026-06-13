---
width: "1920"
---
# AI Fundamentals
# Pertemuan 2
## Miskonsepsi Istilah AI

---
### Permasalahan 
#### Istilah AI muncul dimana-mana, bahkan di tempat yang tidak seharusnya

#### Semantic Satiation <!-- element class="fragment"  -->
Semantic satiation is a psychological phenomenon in which repetition causes a word or phrase to temporarily lose meaning  for the listener. <!-- element class="fragment"  -->

Sebuah fenomena psikologi yang terjadi jika seseorang mengulangi kata yang sama mengakibatkan kata tersebut kehilangan arti.<!-- element class="fragment"  -->

---


![[Ryzen-AI-PRO-9HX-Badge.webp]]


---

![[maxresdefault.jpg]]
---

![[PDP01_1280x.webp]]

---

<!-- slide bg="https://media.tenor.com/x6seeFcZdGMAAAAM/eye-roll-robert-downey-jr.gif" data-background-size="50%" -->

---

## Miskonsepsi

Di kehidupan kita se hari-hari, ketika orang berbicara tentang AI, seringkali yang dimaksud adalah ChatGPT, Gemini, atau Claude.  

Secara spesifik, aplikasi tersebut termasuk kategori subset **Generative AI (GenAI)** atau **Large Language Model (LLM)**, yaitu AI yang dapat menghasilkan data baru (text, image, audio) berdasarkan data yang sudah dipelajari sebelumnya. 


---

![[1724961945965 1.jpeg]]

spoiler: kita akan belajar tentang semua ini secara lebih detil di pertemuan selanjutnya

---
#### GenAI (Generative AI) melibatkan bidang-bidang:

**Machine Learning**, sebuah sistem yang mampu mempelajari pola dari data yang sudah ada dan dapat membuat kesimpulan akurat tentang data yang baru - [IBM](https://www.ibm.com/think/topics/machine-learning) 

**Deep Learning**, sebuah sistem yang menggunakan neural network, mirip otak manusia, yang digunakan untuk mempelajari fitur atau pola dari data yang sangat besar. Deep learning adalah sistem inti dari produk LLM seperti ChatGPT dan Gemini -[IBM](https://www.ibm.com/think/topics/deep-learning) 

**Natural Language Processing**, sistem komputer yang dapat membaca dan memahami tulisan dan bahasa natural manusia. Contoh: Autocorrect

---

**Computer Vision**, sistem komputer yang dapat melihat dan menganalisa informasi visual dari gambar atau video. Contoh: Heat Camera, Sensor Deteksi Api, Facial Recognition (Windows Hello/ Apple unlock)

Contohnya:

![[computer-vision-problems-v0-zoy69bcgvocd1.webp]]<!-- element class="fragment"  -->

---

**Audio Processing**, teknik komputer yang digunakan untuk menganalisa, memahami dan memanipulasi sinyal audio dari musik atau suara manusia. Sistem dapat membedakan suara manusia dan suara bukan manusia. Contoh: Whatsapp, Discord, Noise Cancelling

Contoh lain:

![[starboy.mp3]]

---

 ![[Gawr_Gura.webp]]


---

## Karakteristik AI
Sebuah product bisa dibilang AI, ketika memenuhi beberapa karakteristik dibawah:
- Belajar dan Adaptasi, Sistem dapat belajar dari data dan pengalaman sebelumnya, dan menggunakan pembelajaran tersebut untuk berkembang.<!-- element class="fragment"  -->
- Penalaran dan Pemecahan Masalah, Sistem dapat membuat sebuah statement berdasarkan data, dan mengambil keputusan untuk menyelesaikan masalah yang kompleks<!-- element class="fragment"  -->
- Persepsi, Sistem dapat mengolah data yang bisa dilihat (teks, gambar, video) dan didengar (musik), layaknya panca indera manusia<!-- element class="fragment"  -->
- Autonomi, Sistem dapat menjalankan fungsi secara otomatis tanpa campur tangan manusia secara terus-menerus<!-- element class="fragment"  -->
- Menangani Ketidakpastian, sistem dapat membuat keputusan yang optimal berdasarkan informasi yang ada, walaupun informasi terkadang tidak lengkap, tidak pasti, atau tidak akurat. <!-- element class="fragment"  -->
- Fokus pada Hasil, sistem di desain untuk mencapai sebuah objektif atau pencapaian khusus dan akan mengoptimalkan hasil berdasarkan target tersebut.<!-- element class="fragment"  -->

---

## Machine Learning (AI) vs Algoritma (Non-AI)

Algoritma bekerja berdasarkan aturan yang ditulis secara langsung oleh manusia<!-- element class="fragment"  -->
Algoritma bersifat deterministik, jika input a, maka output a, tidak pernah berbeda<!-- element class="fragment"  -->

AI/machine learning bekerja berdasarkan pola yang dipelajari dari data training<!-- element class="fragment"  -->
probabilistik, jika input a, kemungkinan output bisa a,b,c tergantung pola yang dipelajari<!-- element class="fragment"  -->

"jika saya terus menggunakan aplikasi ini, apakah aplikasi akan lebih efisien dalam tugasnya tanpa seorang developer memberikan update?"<!-- element class="fragment"  -->

---

![[Pasted image 20251104114659.png]]

---

![[Pasted image 20251104114713.png]]


---

## Studi Kasus : Google Map

## Apakah Google Map termasuk AI? <!-- element class="fragment"  -->  


---

### Apa masalah yang kita punya? 
- tidak tahu jalan atau rute ke suatu tujuan <!-- element class="fragment"  -->
- jalan atau rute mana yang tercepat ke tujuan <!-- element class="fragment"  -->
- tidak tahu berapa lama durasi perjalanan <!-- element class="fragment"  -->
- tidak tahu seberapa jauh perjalanan <!-- element class="fragment"  -->


---
<style>
	.container{
		width:700px
	}
</style>
### Bagaimana cara menyelesaikan masalah tersebut? 
(fokus pada fitur navigasi)

![[www.google.co_.uk_maps_dir___@51.5232166-1.08250118z_hlENiPad-Mini.png||400]]<!-- element class="container fragment"  --> 
- mapping gambar satelit ubah tikungan/persimpangan menjadi titik (node) <!-- element class="fragment"  -->
- buat jalan antara titik tersebut (vertex) <!-- element class="fragment"  -->
- berikan nilai "resistansi" terhadap jalan/vertex. semakin panjang, nilai membesar. semakin mulus jalan, nilai mengecil<!-- element class="fragment"  -->
- hitung jalur dengan jumlah resistansi terkecil<!-- element class="fragment"  -->

---

### Hasilnya?

![[Pasted image 20251103133607.png]]<!-- element class="fragment"  -->


---
#### apakah algoritma dapat memecahkan masalah secara rasional?

YA, karena permasalahan utama, yaitu mencari rute tercepat dapat diselesaikan dengan baik oleh algoritma. <!-- element class="fragment"  -->


---
## Apakah algoritma dapat "melihat" data? 
 
 <iframe width="560" height="315" src="https://www.youtube.com/embed/Q_ymY_8ffLo?si=D2u20AwQnZ7ATApU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### Bagian mana yang dimaksud dengan "data"?  <!-- element class="fragment"  -->
jalan sebagai vertex, tikungan sebagai node <!-- element class="fragment"  -->


---

#### Jenis data apa saja yang dilihat oleh google maps?

data actual nya yaitu gambar bumi dari satelit, jenis data visual <!-- element class="fragment"  -->
selanjutnya data visual diubah menjadi data angka, lalu dihitung, dan di informasikan ke user <!-- element class="fragment"  -->

YA, algoritma bisa melihat data <!-- element class="fragment"  -->

---
#### apakah algoritma dapat menangani ketidakpastian?
jika kita memilih jalan yang salah,? <!-- element class="fragment"  -->

maka aplikasi akan meng-update rute terdekat. <!-- element class="fragment"  -->

Jika tidak ada rute di depan?<!-- element class="fragment"  -->

maka pengendara akan disuruh putar balik. <!-- element class="fragment"  -->

Terkadang jalan yang dipilih oleh google maps terlalu kecil untuk kendaraan, terutama jalanan di pinggiran kota. Fungsi ini juga mencakup autonomi dan fokus pada hasil. <!-- element class="fragment"  -->

---
#### apakah algoritma navigasi (hanya navigasi) dapat belajar ?

 TIDAK, algoritma hanya bisa di optimasi. <!-- element class="fragment"  -->
 
contohnya, sebuah mobil yang mempunyai kecepatan maksimal 300kmh, untuk mencapai kecepatan yang lebih dari 300kmh, mobil harus berhenti berjalan dan diubah settingan mesin, ganti jenis ban, pasang bodykit, etc. Tidak mungkin mobil akan belajar sendiri cara menjadi lebih cepat. <!-- element class="fragment"  -->

---

### apakah termasuk AI?
TIDAK,  jika kita hanya membahas tentang algoritma dijkstra, algoritma ini termasuk classical algorithm, dan dapat digunakan di bidang lain, contohnya network. <!-- element class="fragment"  -->

Namun di aplikasi google maps yang modern, algoritma ini dapat digunakan bersama sistem AI, contohnya, prediksi kemacetan <!-- element class="fragment"  -->

https://blog.google/products/maps/google-maps-101-how-ai-helps-predict-traffic-and-determine-routes/ <!-- element class="fragment"  -->

---

### Apakah Google Maps membantu kita di kehidupan sehari-hari?
pasti <!-- element class="fragment"  -->

---
### Kesimpulan
ChatGPT, Gemini, Claude, dll bisa dipanggil AI, namun lebih cocok atau akurat jika dipanggil Large Language Model atau Generative AI (GenAI)<!-- element class="fragment"  -->

Sistem yang bukan termasuk AI bisa terlihat sangat pintar dan canggih, dan tentu sangat membantu kehidupan kita.<!-- element class="fragment"  -->