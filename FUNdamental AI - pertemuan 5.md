---
width: "1900"
---
# Pertemuan 5
# Batasan-batasan dari AI

---

## Kemampuan Machine Learning

Kemampuan machine learning didapatkan oleh jenis dataset dan proses training.

Mirip dengan manusia, kita mendapatkan kemampuan atau skill berdasarkan pelajaran yang kita dapatkan dari sekolah atau pengalaman.  <!-- element class="fragment"  -->

Oleh karena itu, manusia dapat melakukan apa saja, kemampuan manusia untuk beradaptasi sangatlah tinggi  <!-- element class="fragment"  -->

---

### Trivia 
Apakah kalian tahu pekerjaan apa yang punya gaji per jam paling tinggi?

masalah utama dari pekerjaan ini adalah tidak banyak orang yang berani menjalaninya <!-- element class="fragment"  -->

![[https://i.natgeofe.com/n/e7f802c7-6e47-4ad0-9168-e24ac480e1cc/GettyImages-1053853578.jpg]]<!-- element class="fragment"  -->

##### Underwater Welding <!-- element class="fragment"  -->

---

## Tugas yang dilakukan Machine Learning

Bagaimana dengan AI? 

Apa saja tugas-tugas yang bisa dilakukan oleh AI? <!-- element class="fragment"  -->

Semua pekerjaan yang dilakukan oleh AI bisa dikategorikan menjadi 3<!-- element class="fragment"  -->

---
### Prediksi / Regresi

![[335415346_711253537457018_7185100068761096947_n.png]]


---

### Klusterisasi 
![[https://developers.google.com/static/machine-learning/clustering/images/clustering_example.png]]

---

### Decision Making

![[https://substackcdn.com/image/fetch/$s_!Ywxi!,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F0cc9ca6d-a73c-47ff-a1a6-b88b7a0b651b_387x585.jpeg]]


---

Dengan mengetahui jenis tugas yang dapat dilakukan oleh Machine Learning, maka kita paham masalah apa yang bisa di selesaikan dan tidak bisa diselesaikan dengan AI.

![[1761861429884.jpeg]]


---

### Regresi atau Prediksi

Machine Learning mempelajari pola yang ada di data, lalu memprediksi sesuatu berdasarkan data yang belum pernah ditemui atau dipelajari <!-- element class="fragment"  -->

Hasil prediksi harus di validasi dengan hal yang ada di dunia nyata atau sesuatu yang sudah pasti benar (ground truth) <!-- element class="fragment"  -->

LLM dan Autocorrect adalah salah satu bentuk Regresi atau Prediksi <!-- element class="fragment"  -->


---

Untuk melatih Machine Learning melakukan tugas ini, kita harus memberikan Labeled Data (data yang mempunyai label) yang bertindak sebagai Ground Truth di proses training 


![[https://labelyourdata.com/img/article-illustrations/4_image_2nd_post.png]]

---
Contoh lain :

![[FaKO4mMXwAERmI_.jpg]]

ini contoh yang salah, prediksi data di excel tidak menggunakan machine learning (mungkin sekarang sudah di update) <!-- element class="fragment"  -->

---

Contoh lain :

#### Harga Tiket Konser

| bintang tamu                               | jumlah kursi | Jumlah fans total | harga tiket  |
| ------------------------------------------ | ------------ | ----------------- | ------------ |
| Blackpink                                  | 5000         | 370juta           | Rp 3.800.000 |
| Maroon5                                    | 1000         | 70juta            | Rp 2.500.000 |
| Reality Club                               | 500          | 3juta             | Rp 250.000   |
| Nadine Amizah                              | 2000         | 10juta            | Rp 500.000   |
| Sheila on 7                                | 3000         | ???               | ???          |
| Reality Club<br>\+ Nadine Amizah<br>+ Noah | ???          | ???               | ???          |

Berapa harga tiket sheila on 7?

berapa harga tiket konser reality club + nadine amizah + noah ? 

Data apa yang dibutuhkan untuk melakukan prediksi?


---
### Klusterisasi

Machine learning mempelajari pola yang ada di data untuk membagi sekumpulan objek ke dalam kelompok-kelompok tertentu.


---

Untuk melatih Machine Learning melakukan tugas ini, kita harus memberikan Unlabeled Data 

![[Pasted image 20251110091939.png]]

Hasil dari klusterisasi juga unlabeled data, tapi sudah terkategorikan / tersortir secara rapi

---
### Sequential Decision / Reinforcement Learning (RL)

Model machine learning membuat serangkaian keputusan dari waktu mulai sampai selesai di dalam lingkungan yang tidak diketahui untuk memaksimalkan nilai akhir (reward) <!-- element class="fragment"  -->

Machine learning akan melakukan proses eksperimen / trial and error. Ketika model mengalami kegagalan, maka model akan mengulang eksperimen kembali secara otomatis <!-- element class="fragment"  -->

---
#### Contoh Natural (manusia)

Ada sebuah pohon belimbing yang tinggi de, anda tidak pernah melihat sebuah pohon belimbing (pura pura aja), tapi anda tahu bahwa anda bisa makan belimbing/buahnya
![[https://previews.123rf.com/images/saiko3p/saiko3p1309/saiko3p130900320/22093375-very-big-jack-fruit-tree-with-fruits.jpg]]

apa reward dari situasi ini?<!-- element class="fragment"  -->

buah belimbing<!-- element class="fragment"  -->

---

Bagaimana cara kita mendapatkan belimbing?

percobaan pertama : loncat <!-- element class="fragment"  -->

![[https://images.unsplash.com/photo-1461800919507-79b16743b257?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8M3x8cGVvcGxlJTIwanVtcGluZ3xlbnwwfHwwfHx8MA%3D%3D&fm=jpg&q=60&w=3000]]<!-- element class="fragment"  -->

ternyata pohon terlalu tinggi<!-- element class="fragment"  -->

---
percobaan kedua: **tangga**<!-- element class="fragment"  -->

![[https://www.badgerladder.com/wp-content/uploads/magictoolbox_cache/ad391aebc1f9913654f3f7c70f89e9ae/5/9/590/original/1160400600/type-1aa-extra-heavy-duty-fiberglass-double-step-ladder-375-pound-capacity-1.jpg]]<!-- element class="fragment"  -->

---
percobaan ketiga: **Alat pemanjat pohon**<!-- element class="fragment"  -->

![[https://indianinovatix.com/wp-content/uploads/2021/10/Coconut-Climber-1.png]]<!-- element class="fragment"  -->

---
Hasilnya?
![[https://media-cdn.tripadvisor.com/media/photo-p/10/d3/d1/0a/eating-star-fruit-straight.jpg]]<!-- element class="fragment"  -->

mantap <!-- element class="fragment"  -->

---
#### Contoh mesin

[alphago](https://deepmind.google/research/alphago/)

[alpha-go vs lee sedol](https://www.youtube.com/shorts/whNvUWRQPhY)

[alphago documentary](https://www.youtube.com/watch?v=WXuK6gekU1Y) 



---

#### Contoh Mesin (2)

OpenAI 5 mengalahkan juara dunia OG

<iframe width="560" height="315" src="https://www.youtube.com/embed/tfb6aEUMC04?si=lKkK5f5yhsOZRMkx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

## Hubungannya dengan LLM

LLM atau autocorrect termasuk dalam tugas .... **prediksi**  <!-- element class="fragment"  -->

karena LLM mendapatkan training data berbentuk teks dan mencari makna dari data tersebut <!-- element class="fragment"  -->

ketika proses training selesai, kita bertanya ke LLM, dan jawaban dari pertanyaan akan di "prediksi" berdasarkan pertanyaan dan pola yang dipelajari <!-- element class="fragment"  -->

memunculkan satu kata sebagai hasil prediksi, <!-- element class="fragment"  -->

lalu prediksi tersebut diulang-ulang sampai jawaban selesai <!-- element class="fragment"  -->

---

## Halusinasi

![[Pasted image 20251110100047.png]]


---

LLM sering berhalusinasi <!-- element class="fragment"  -->

Halusinasi adalah hasil dari faktualitas (kemampuan mengikuti fakta) dan creativitas (kemampuan untuk membuat sesuatu yang original) <!-- element class="fragment"  -->

Halusinasi dapat dikurangi, tapi tidak dapat dihilangkan secara penuh <!-- element class="fragment"  -->

Cara untuk mengurangi halusinasi adalah dengan membandingkan hasil prediksi dengan data yang ada di dunia nyata (deep search) <!-- element class="fragment"  -->

---
Contoh

AWS mengalami gangguan/outage di salah satu server paling besar nya, mengakibatkan setengah dari internet lumpuh sementara. Report ini menjelaskan kronologi gangguan, kemungkinan besar dibuat oleh AI. (sudah di revisi)

![[Pasted image 20251110101013.png]]

---

contoh lain

![[https://assets.zilliz.com/An_Example_of_Intrinsic_vs_Extrinsic_Hallucination_bcbd635c1b.png]]

---

## Context Rot

![[Pasted image 20251110103012.png]]

---

#### Token

token adalah satuan unit yang digunakan oleh LLM untuk memproses data. 

100 token = 60-80 kata  <!-- element class="fragment"  -->

aku makan nasi padang = 4 token <!-- element class="fragment"  -->

Sebagai contoh, google gemini mempunyai 1 juta token limit untuk input <!-- element class="fragment"  -->

![[Pasted image 20251110103439.png]]<!-- element class="fragment"  -->

---
#### Hasil temuan dari riset

1. Semakin banyak token input yang diberikan, maka hasil/akurasi LLM semakin jelek<!-- element class="fragment"  -->

![[hero_plot.png]]

---

2. Kompleksitas pekerjaan dan instruksi yang ambigu juga memperjelek akurasi LLM<!-- element class="fragment"  -->

![[needle_question_sim_arxiv.png]]


---

3. jika ada sebuah "distractor", data yang mirip dengan hasil, tapi bukan hasil, maka akurasi akan jauh lebih jelek

contoh distractor: 
![[distractor_irrelevance.png]]

---

akurasi LLM dengan distractor

![[distractors_num.png]]


---
#### Solusi

Kita harus melakukan "context engineering", yaitu memberikan struktur dan data yang tepat untuk prompt input, agar semua data dapat di cerna oleh LLM secara sempurna dan kita mendapatkan hasil yang akurat.

kita akan mempelajari topik ini secara lebih dalam di pertemuan selanjutnya

---

## Bias and Subjectivity

Bias atau prasangka atau stereotype adalah kecenderungan untuk lebih menyukai satu orang atau sesuatu daripada yang lain, dan lebih memihak pada orang atau sesuatu tersebut.

faktor utama dari bias adalah hal yang kita alami atau temui sehari-hari <!-- element class="fragment"  -->


---
#### contoh natural 

Bayangkan gambar seorang perawat di kepala anda.

apakah perawat tersebut laki laki atau perempuan? <!-- element class="fragment"  -->

kita punya bias terhadap perawat perempuan, karena ketika kita ke rumah sakit, sebagian perawat yang kita temui adalah perempuan <!-- element class="fragment"  -->

---

#### Contoh machine learning

Jika kita memberikan prompt "buatlah gambar dari penemu bangsa amerika", kira-kira gambar apa yang akan kita dapatkan?

![[https://pbs.twimg.com/media/GG3FzlWW4AAtZ4d?format=jpg&name=small]]<!-- element class="fragment"  -->


---

Jika kita memberikan prompt "buatlah gambar seorang viking", kira-kira gambar apa yang akan kita dapatkan?

![[https://pbs.twimg.com/media/GG3FzlYXoAAriL_?format=jpg&name=360x360]]<!-- element class="fragment"  -->

---

Bias terjadi karena data training yang tidak seimbang, atau label dari data yang kurang pas, atau informasi yang bersifat misleading di dalam training data.

sama saja dengan perawat yang kita temui, realitanya memang perawat perempuan jauh lebih banyak dari perawat laki laki<!-- element class="fragment"  -->

![[Pasted image 20251110112906.png]]
![[Pasted image 20251110112923.png]]


---

# berita hangat


![[Pasted image 20251110112711.png]]

---

![[Pasted image 20251110112727.png]]

---

| Institution               | AI bias                | Year | Example                                                                                                                                                                                   | Results                                                                                                                                                                |
| ------------------------- | ---------------------- | ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Study on AI in Healthcare | Racism                 | 2021 | AI-driven diagnostic tools for skin cancer are less accurate for individuals with dark skin due to lack of diversity in training datasets.                                                | Misdiagnosis risk for individuals with darker skin tones; exclusion from AI-based clinical applications due to insufficient representation in training data.           |
| Healthcare Risk Algorithm | Racism                 | 2019 | A healthcare risk-prediction algorithm used on over 200 million U.S. citizens favored white patients over black patients.                                                                 | The algorithm relied on healthcare spending as a proxy for medical needs, leading to inaccurate predictions and racial bias due to correlated income and race metrics. |
| MIT Technology Review     | Sexism                 | 2022 | Lensa AI avatar app produced sexualized images of Melissa, an Asian woman, without consent, while male colleagues received empowering images.                                             | AI perpetuated gender and racial stereotypes, highlighting issues in biased training data and developer decisions.                                                     |
| Amazon                    | Sexism                 | 2015 | Amazon’s AI recruiting tool showed bias against women by penalizing resumes that included the word “women’s.”                                                                             | The AI system incorrectly learned that male candidates were preferable due to biased historical data, leading Amazon to discontinue the use of the algorithm.          |
| Facebook                  | Sexism and Racial Bias | 2019 | Facebook allowed advertisers to target ads based on gender, race, and religion, showing women nursing roles and men janitorial roles, often targeting minority men for lower-paying jobs. | Due to these biases, Facebook stopped allowing employers to specify age, gender, or race targeting in ads, acknowledging the bias in its ad delivery algorithms.       |

---

## Computing Power

https://www.nucnet.org/news/microsoft-backed-fusion-company-begins-work-on-washington-nuclear-fusion-plant-7-4-2025

---
