---
width: "1920"
---
# Definisi LLM

Adakah yang masih ingat dengan definisi Algoritma? <!-- element class="fragment"  -->
Algoritma adalah sekumpulan instruksi untuk melakukan pekerjaan <!-- element class="fragment"  -->

Apa hubungannya dengan LLM, atau Large Language Model? <!-- element class="fragment"  -->
Pertama-tama, kita belajar tentang arti dari "Model" dulu <!-- element class="fragment"  -->

---

## Apa definisi dari Model? 

ini?<!-- element class="fragment"  -->

![[1001533164.webp]]
<!-- element class="fragment"  -->
bukan ya 😅<!-- element class="fragment"  -->

---

Model adalah sebuah program yang dapat menemukan atau menganalisa pola dan membuat keputusan setelah memproses data

![[Pasted image 20251105103635.png]]

---
#### Salah satu jenis Model, yaitu model deteksi objek

![[https://images.prismic.io/encord/2c542f46-1b16-4696-98bc-a4a83bf682fe_image1.jpg?auto=compress,format]]

Apa input dari model? <!-- element class="fragment"  -->
Apa output dari model? <!-- element class="fragment"  -->

---

### Large Language Model (LLM) adalah... 
jenis model yang dilatih/ditraining dengan data teks yang berjumlah sangat besar (Large) <!-- element class="fragment"  -->

sehingga model bisa memahami, memproses bahasa yang digunakan oleh manusia (Language) <!-- element class="fragment"  -->

dan menghasilkan teks yang bisa dimengerti oleh manusia (Model). <!-- element class="fragment"  -->

LLM adalah salah satu pengaplikasian dari Generative AI. <!-- element class="fragment"  -->


![[Pasted image 20251105101528.png]]

---

### Bagaimana cara LLM bekerja?
LLM menjawab pertanyaan kita dengan memprediksi kata berikutnya yang akan muncul, terus menerus, sampai jawaban selesai. <!-- element class="fragment"  -->
kedengarannya mirip dengan teknologi yang sudah ada sejak awal tahun 2000.... <!-- element class="fragment"  -->

![[https://images.samsung.com/is/image/samsung/assets/uk/support/mobile-devices/how-can-i-personalise-and-turn-predictive-text-on-and-off-on-my-samsung-galaxy-device/images/1-uk-how-can-i-personalise-and-turn-predictive-text-on-and-off.png?$ORIGIN_PNG$]]<!-- element class="fragment"  -->

---

# LLM vs Autocorrect/Predictive Text

Autocorrect terdiri dari dua komponen:

Jika kita salah mengetik suatu kata, autocorrect akan secara otomatis mengubah kata tersebut menjadi versi yang benar (autocorrect) <!-- element class="fragment"  -->

Ketika kita mengetik suatu huruf, maka keyboard akan memprediksi hurut tersebut akan menjadi kata apa. (predictive text) <!-- element class="fragment"  -->

Saat ini, kita akan fokus lebih ke fitur predictive text <!-- element class="fragment"  -->

![[https://images.samsung.com/is/image/samsung/assets/uk/support/mobile-devices/how-can-i-personalise-and-turn-predictive-text-on-and-off-on-my-samsung-galaxy-device/images/1-uk-how-can-i-personalise-and-turn-predictive-text-on-and-off.png?$ORIGIN_PNG$]]<!-- element class="fragment"  -->

---

## Cara Kerja Predictive Text

lengkapi kalimat ini:

#### Merah kuning hijau, di langit yang ..... <!-- element class="fragment"  -->

mendung? <!-- element class="fragment"  -->

indah? <!-- element class="fragment"  -->

![[Pasted image 20251105111713.png]]<!-- element class="fragment"  -->

biru? <!-- element class="fragment"  -->

---

berapa probabilitas untuk masing masing jawaban? 

mendung =3%<!-- element class="fragment"  -->

indah = 2%<!-- element class="fragment"  -->

biru = 95%<!-- element class="fragment"  -->

kenapa biru bisa 95%? bagaimana cara autocorrect menentukan angka 95%? <!-- element class="fragment"  -->

---

#### Autocorrect adalah bentuk machine learning model yang sederhana
Langkah Pertama : Kumpulkan teks yang akan dibuat training, contohnya sebuah novel.
![[https://images.unsplash.com/photo-1541854615901-93c354197834?fm=jpg&q=60&w=3000&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1yZWxhdGVkfDE5fHx8ZW58MHx8fHx8]]

---
Langkah Kedua : tentukan frekuensi dari pasangan kata
![[https://figures.semanticscholar.org/dda43b361b7d893e141cc3153bf9d4f64619a6d5/22-Table1.1-1.png]]

Jika frekuensinya besar, maka probabilitasnya tinggi <!-- element class="fragment"  -->

---
Elections are to take ....
- place (terjadi) 92%
- account (tanggung jawab) 5%
- flight (terbang) 3%

---

Cukup simpel kan? hanya 3 langkah 

Perbedaan Autocorrect dengan LLM 
- dataset LLM jauh lebih besar<!-- element class="fragment"  -->
- proses training jauh lebih kompleks <!-- element class="fragment"  -->
- hasil dari LLM jauh lebih baik <!-- element class="fragment"  -->

Namun, secara garis besar, metode nya sama, LLM dan Autocorrect sama-sama memprediksi kata selanjutnya di sebuah kalimat <!-- element class="fragment"  -->

hanya skala dan kompleksitas nya berbeda <!-- element class="fragment"  -->

---
# Dataset dan Proses Training

Perbedaan utama antara LLM dan Autocorrect adalah di dataset dan proses training <!-- element class="fragment"  -->

Dataset adalah data berbentuk teks (atau bentuk lain) yang akan dipelajari oleh sebuah model.<!-- element class="fragment"  -->

---


Di dunia machine learning, ada satu quote yang sangat penting, yaitu <!-- element class="fragment"  -->

## `Garbage in, garbage out` <!-- element class="fragment"  -->

![[https://www.shutterstock.com/image-vector/garbage-in-out-gigo-concept-260nw-2356548575.jpg]]<!-- element class="fragment"  -->

Artinya, jika input dari model jelek, maka output dari model sudah pasti jelek <!-- element class="fragment"  -->

Manusia pun mirip, jika makanan berkualitas rendah, maka performa manusia menurun <!-- element class="fragment"  -->


---

Kita akan mempelajari proses pemilihan dataset dan training menggunakan analogi yang kalian pasti bisa relate <!-- element class="fragment"  -->

#### murid yang sedang belajar sebelum menghadapi ujian akhir  <!-- element class="fragment"  -->

---
## 1. Pengumpulan Sumber Data

| Konsep                                                                                       | Analogi                                                                                             |
| -------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Pengumpulan data. Data ini terdiri dari jutaan, bahkan milyaran artikel, jurnal, dan website | Mahasiswa membeli buku-buku yang perlu dipelajari, mengatur jadwal, dan membatalkan rencana healing |

![[https://cdn.mos.cms.futurecdn.net/6c3s8rMup3oTAUKywn4UTT.jpg]]

---
#### Dari mana saja data diambil?
dari semua material di internet yang dapat diakses oleh semua orang (public), antara lain:

---
##### Paper/Jurnal (sumber utama)
arxiv.org

![[Pasted image 20251105140116.png]]
dalam proses training, LLama 70b (LLM buatan google) mampu memproses 1000 paper per menit <!-- element class="fragment"  -->
(paper ini adalah terobosan utama yang memungkinkan chatgpt 3 menjadi sangat 'pintar') <!-- element class="fragment"  -->

---
##### Sosial Media untuk sumber opini
##### Facebook 
##### Reddit
##### Twitter 

---
##### Forum tanya jawab
##### Quora
##### Brainly

##### Stackoverflow
##### Kaskus

---

##### Article Tech
##### Medium
##### AndroidCentral
##### 9to5Linux

---
##### Tutorial Tech

##### GeekToGeeks
##### Instructables

---

##### Edukasi
##### Khanacademy
##### EnglishFirst

##### Duolingo


---

##### Berita Dunia
##### CNN News
##### BBC News
##### DetikNews

Dan masih banyak lagi

---

## 2. Pre-training

| Konsep                                                                                                                | Analogi                                                                                                                      |
| --------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| LLM membaca dan menganalisa jutaan, bahkan milyaran artikel, jurnal, dan website. Hasilnya adalah sebuah "Base Model" | Mahasiswa mempelajari setumpukan buku-buku tentang materi yang akan diajarkan di ujian akhir dan mengikuti sesi latihan soal |

![[https://nolafamily.com/wp-content/uploads/2016/09/photodune-8482868-frustrated-pretty-student-studying-between-piles-of-books-in-library-l-scaled.jpg]]

---
Proses ini mirip dengan proses training autocorrect yang telah dijelaskan,  

namun skala datasetnya jauh lebih besar <!-- element class="fragment"  -->

dan banyak langkah2 tambahan di proses trainingnya<!-- element class="fragment"  -->

---
## 3. Proses Training

| Konsep                                                                                                    | Analogi                                                                                                                                                 |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| LLM di test dengan data yang kualitasnya sangat amat tinggi. Kemungkinan besar skor hasil test nya rendah | Mahasiswa mengikuti ujian tengah semester, dan gagal. Tingkat stres meningkat. Namun Mahasiswa mendapatkan ilmu baru karena dosen memberi kunci jawaban |

![[https://solportal.ibe-unesco.org/wp-content/uploads/2021/02/exams-stress.jpg]]

detil dari proses training akan dipelajari di pertemuan 9-10<!-- element class="fragment"  -->

---

## 4. Reinforcement Learning

| Konsep                                                                                                                                                                                                                                                                                                                   | Analogi                                                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| LLM di test dengan bantuan manusia. Manusia bertanya dan LLM akan menjawab. Manusia akan memberi review/rating jawaban tersebut, dari skala 0-10. LLM akan mencerna review ini dan menjawab pertanyaan selanjutnya berdasarkan feedback yang diterima. Teknik ini dinamakan RLHF (Reinforcement Learning Human Feedback) | Mahasiswa menyewa guru privat yang sangat mahir dibidangnya dan punya 10 tahun pengalaman. Mahasiswa melakukan latihan soal dengan guru les privat. Guru les privat memberi tahu mahasiswa jawaban mana yang lebih baik/benar. |

![[https://clueylearning.com.au/wp-content/uploads/2019/10/What-is-tutoring-Different-types-of-tutoring-explained.jpg]]


---

## 5. Model Evaluation / Benchmark

| Konsep                                                                                                  | Analogi                                                                                    |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Dilakukan proses testing yang banyak dan mendetil. Gunanya untuk mengukur kemampuan LLM secara general. | Mahasiswa mengikuti Ujian Akhir yang menentukan nasib Mahasiswa. Dan mahasiswa bisa lulus! |
|                                                                                                         |                                                                                            |

![[https://images.ctfassets.net/mrbo2ykgx5lt/24042/020297b25ffce8398280cb06da0cecb5/psychology-academic-achievement-good-exam-results.jpg]]

---

Di proses training yang nyata, ketika skor benchmark masih rendah, maka LLM akan di-training ulang, kembali ke langkah nomor 3.

Proses ini di ulang-ulang sampai LLM mencapai target skor benchmark.

---

# Kemampuan yang muncul

Karena perbedaan skala data dan kompleksitas proses training jika dibandingkan oleh model autocorrect, maka beberapa sifat atau kemampuan muncul dengan sendirinya, antara lain:

![[Pasted image 20251105150904.png]]

---

## *Emergence is when quantitative changes in a system result in qualitative changes in behavior*
-Nobel prize-winning physicist Philip Anderson (1972)

#### "kemunculan" terjadi ketika perubahan kuantitatif (skala/jumlah) di sebuah sistem menghasilkan perubahan perilaku yang kualitatif<!-- element class="fragment"  -->

---

### Prompting
Perbedaan utama LLM dan Autocorrect adalah kita dapat berinteraksi dengan LLM

berinteraksi maksudnya kita bisa berbicara layaknya seorang manusia (chatbot), dan memberikan instruksi yang dapat dikerjakan oleh LLM <!-- element class="fragment"  -->

![[468298818_10162082691996878_5552546406547739701_n.jpg]]<!-- element class="fragment"  -->

---

### Reasoning (Penalaran)
LLM mempunyai kemampuan logika yang cukup signifikan jika dibandingkan dengan autocorrect. 

LLM adalah salah satu teknologi buatan manusia yang bisa melakukan pemikiran logika secara general.<!-- element class="fragment"  -->

Namun tetap saja, kemampuan general reasoning manusia jauh lebih maju, terutama jika kita melihatnya secara kualitatif. <!-- element class="fragment"  -->

"is there a seahorse emoji" <!-- element class="fragment"  -->

![[https://prompt.16x.engineer/nextImageExportOptimizer/wrong-answer.4536ac48-opt-1920.WEBP]]<!-- element class="fragment"  -->


---
## Coding (Bahasa Programming)

Awalnya LLM hanya ditujukan untuk pembelajaran bahasa natural manusia, seperti bahasa inggris, indonesia, etc

namun, karena ada data tentang code di dataset ([stackoverflow](https://stackoverflow.com/questions/6211613/testing-whether-a-value-is-odd-or-even)), ternyata LLM bisa mempelajari bahasa programming juga. 

menggunakan LLM/AI untuk membuat code namanya "Vibe Coding" <!-- element class="fragment"  -->

![[ai-coding-v0-xp7jvaw54sld1.webp]]

---

# The Big Players 

| Model        | Perusahaan Pengembang | Filosofi / Fokus Utama      | Keunggulan yang Diklaim                                                               |
| ------------ | --------------------- | --------------------------- | ------------------------------------------------------------------------------------- |
| **ChatGPT**  | OpenAI                | Aksesibilitas & Kapabilitas | Dialog yang alami, kreativitas, kekuatan serba bisa                                   |
| **Gemini**   | Google / DeepMind     | Integrasi & Multimodalitas  | Terintegrasi dengan ekosistem Google, pemahaman _native_ atas gambar/video            |
| **Claude**   | Anthropic             | Keamanan & Etika            | Sangat aman, jendela konteks besar (analisis dokumen panjang), terbaik untuk ngoding. |
| **DeepSeek** | DeepSeek AI           | Demokratisasi & Efisiensi   | _Open-source_, efisiensi biaya, kemampuan _coding_ & penalaran yang kuat              |


---

# Tipe LLM

LLM adalah produk yang sangat populer. Kita akan mempelajari berbagai macam jenis LLM yang muncul.

---
## Berdasarkan Training Data - General Purpose

Model "serba bisa" yang Anda kenal, seperti GPT-4 atau Claude 3. Mereka dilatih pada data internet yang sangat luas dan dirancang untuk menangani jutaan tugas berbeda, mulai dari menulis puisi hingga meringkas artikel.

|     Kekuatan      |                                                       Kelemahan                                                       |
| :---------------: | :-------------------------------------------------------------------------------------------------------------------: |
| Sangat fleksibel. | Mungkin tidak akurat ketika dihadapkan pada jargon teknis yang sangat spesifik atau pengetahuan domain yang mendalam. |

---

## Berdasarkan Training Data - Domain Specific LLM 

Ini adalah model yang dilatih secara khusus untuk satu bidang industri. Sebagian besar data juga berasal dari bidang industri yang sama

|                                                  Kekuatan                                                   |              Kelemahan               |
| :---------------------------------------------------------------------------------------------------------: | :----------------------------------: |
| Memiliki akurasi, presisi, dan pemahaman konteks yang jauh lebih tinggi di dalam domain spesialisasi mereka | Tidak berguna di luar domain mereka  |

Contoh : https://sites.research.google/med-palm/<!-- element class="fragment"  -->

Contoh yang lebih spesifik: https://deepmind.google/science/alphafold/<!-- element class="fragment"  -->

---
## Berdasarkan Jenis Copyright - Open Source

LLM tipe open source dapat dipakai oleh siapa saja, dengan kepentingan apapun.

Selain itu, dataset, proses training, hasil model, dan semua code yang digunakan bisa dilihat dan diakses oleh siapa saja, memungkinkan programmer dari seluruh penjuru dunia untuk mengembangkan project nya  <!-- element class="fragment"  -->

Deepseek adalah sebuah perusahaan berasal china yang mempunyai fokus untuk membuat LLM yang efisien/hemat dan open source<!-- element class="fragment"  -->

salah satu produk unggulan nya adalah [Deepseek R1](https://github.com/deepseek-ai/deepseek-LLM)yang bisa dijalankan di PC atau laptop dengan spek mid-high (lebih dr 10jt) <!-- element class="fragment"  -->

---

##  Berdasarkan Jenis Copyright - Closed Source

LLM closed source contohnya adalah hampir semua produk LLM yang kita gunakan, dari chatgpt, gemini, dan claude.

closed source bisa diartikan menjadi "rahasia perusahaan", jadi tidak ada orang yang boleh melihat selain pekerja perusahaan <!-- element class="fragment"  -->


---

## Berdasarkan Input Data - Multimodal

LLM umumnya hanya menerima data dalam bentuk teks

Namun banyak terobosan baru yang memungkinkan LLM untuk menerima data gambar, menganalisa dan mengambil makna dari gambar tersebut, lalu diubah menjadi teks, dan di cerna oleh LLM  <!-- element class="fragment"  -->

Jadi kita tidak perlu mendeskripsikan benda yang kita maksud, cukup kirim foto atau gambar dari barang tersebut  <!-- element class="fragment"  -->

Selain gambar, LLM juga bisa menerima informasi dalam bentuk audio <!-- element class="fragment"  -->

Masih menggunakan teknologi transformer yang sama, data audio diubah menjadi data teks, dan dicerna oleh LLM <!-- element class="fragment"  -->

Karena LLM ini membutuhkan data dan proses training yang cukup spesial, maka hanya ada beberapa model yang bisa melakukan ini, contohnya chatgpt dan gemini <!-- element class="fragment"  -->

---

Kenapa meta tidak membuat multimodal LLM?

<iframe width="560" height="315" src="https://www.youtube.com/embed/I5_JrfvO4G8?si=slBVbcuPaMNaI55H" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe><!-- element class="fragment"  -->

mereka sudah membuatnya, tapi hasilnya sangat kurang jika dibandingkan dengan chatgpt dan gemini <!-- element class="fragment"  -->

---
## Berdasarkan Teknik Inferencing - Deep Research

https://gemini.google/overview/deep-research/