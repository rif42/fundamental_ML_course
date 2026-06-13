---
width: "1920"
---
# Pertemuan 6
# Teknik Prompting LLM

---

## Emergent Abilities

Masih ingat kemampuan yang muncul di LLM karena skala data training yang sangat besar?

Salah satu dari kemampuan yang muncul tersebut adalah.. 
#### prompting  F


---

## Apa itu Prompting?

prompting adalah proses interaksi manusia dengan LLM menggunakan bahasa natural untuk mendapatkan sebuah output. <!-- element class="fragment"  -->


---

## Tipe Data

Di proses prompting, ketika kita membuka ChatGPT, kita memberikan sebuah input ke LLM. 

apa jenis data dari input tersebut?  <!-- element class="fragment"  -->

---
## Teks

<!-- slide bg="https://media.tenor.com/sWAbDn43REcAAAAM/imostergolfra.gif" data-background-size="75%" --> 

---
### Teks

Teks adalah jenis input utama yang di cerna oleh LLM.

Karena salah satu media bahasa adalah teks <!-- element class="fragment"  -->

Teks yang didapat akan diubah menjadi token, lalu di proses <!-- element class="fragment"  -->

---

## Gambar

![[https://i1.sndcdn.com/artworks-YDQOy2Pru5CA2rhs-x1uzgA-t500x500.jpg]]


---

## Docs

![[https://www.getyourcv.net/wp-content/uploads/2023/05/professional-cv-template-word.jpg]]

---

## Prompt Engineering

Adalah sebuah metode untuk mendapatkan hasil yang optimal dari LLM dengan mengontrol struktur informasi yang diberikan ke LLM sebagai input. 

Prompt engineering sangat relate dengan ilmu komunikasi <!-- element class="fragment"  -->

Jika terdapat kesalahan dalam berkomunikasi, maka hasil dipastikan akan jelek, apapun tugasnya <!-- element class="fragment"  -->

inilah yang menjadi "bottleneck" interaksi antara LLM dan manusia <!-- element class="fragment"  -->

Tidak hanya itu, prompt engineering dapat mengurangi kelemahan terbesar LLM, yaitu ....<!-- element class="fragment"  -->

---
## Halusinasi

![[spongebob-rainbow.jpg]]

---
### *Garbage in, Garbage out*

### *Garbage question = garbage answer*<!-- element class="fragment"  -->

Inilah kenapa manusia masih dibutuhkan <!-- element class="fragment"  -->

---
#### Studi kasus:

Ada 2 orang yang sedang mempelajari tentang konsep arsitektur brutalisme untuk kepentingan masing masing

asumsinya kedua orang tidak tahu tentang ilmu ini sebelumnya

kedua orang akan belajar dari chatGPT tanpa bantuan sumber lain

---

orang 1, sebut saja Mawar,

![[Pasted image 20251113135040.png]]

seorang programmer php <!-- element class="fragment"  -->

mobil nya lamborghini huracan <!-- element class="fragment"  -->
 
tidak tahu apa apa tentang arsitektur <!-- element class="fragment"  -->

pengen bikin rumah pake estetik brutalisme (duitnya kebanyakan) <!-- element class="fragment"  -->

---

orang 2, sebut saja Danu, 

![[Pasted image 20251113135527.png]]

sudah bekerja sebagai arsitek selama 5 tahun.<!-- element class="fragment"  -->

Ingin mempelajari brutalisme karena klien nya sering lihat tour rumah pake estetik brutalisme<!-- element class="fragment"  -->

punya 3 kucing <!-- element class="fragment"  -->

---

#### kira kira siapa yang bisa mempelajari ilmu estetik brutalisme lebih cepat dan akurat?

kenapa milih Danu?<!-- element class="fragment"  -->

---

##### Kesimpulannya, Kita harus pandai bertanya

Tidak cuma kepada AI, tapi kepada siapapun, dimanapun, kapanpun <!-- element class="fragment"  -->

Karena pandai bertanya adalah salah satu karakteristik orang pintar <!-- element class="fragment"  -->

Bagaimana cara bertanya dengan pintar?<!-- element class="fragment"  -->

---

yang pertama adalah anda butuh CRITICAL THINKING <!-- element class="fragment"  -->

![[https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExNWtsenBncG1tdHk1cGwwb3pxbWZ5M25zNHdqazh4OXVnbmxvcmJlciZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/d3mlE7uhX8KFgEmY/giphy.gif]]


---

yang kedua anda butuh teknik dan struktur <!-- element class="fragment"  -->

yang ketiga anda butuh pengalaman atau pemahaman konteks yang didapatkan dari proses belajar atau pengalaman hidup <!-- element class="fragment"  -->


---
### Basic Prompting  

Seperti halnya berkomunikasi dengan seseorang, ketika kita bertanya dengan AI, kita harus memperhatikan beberapa hal ini:

- Jelas dan Akurat
- Spesifik
- Konteks lengkap

---

asumsikan anda sedang melakukan riset sebelum membeli motor untuk PP rumah-sccr 50km

bagaimana cara anda menanyakan hal tersebut ke LLM?<!-- element class="fragment"  -->

`buatlah sebuah report tentang motor terbaik di indonesia` <!-- element class="fragment"  -->


bagaimana dengan ini :<!-- element class="fragment"  -->

`buatlah sebuah report tentang motor terbaik di indonesia, kategorikan berdasarkan harga, mulai dari entry level, mid level, dan high end. masing-masing kategori, berikan minimal 2 rekomendasi, dan sebutkan kelebihan dan kelemahannya` <!-- element class="fragment"  -->

---

![[Pasted image 20251113141049.png]]


---

### Prompting Element

Jika kita mempunyai pertanyaan yang lebih luas, dan membutuhkan jawaban yang lebih akurat, maka kita harus mengubah strategi prompting kita.

Kita harus menambahkan struktur ke dalam prompt kita <!-- element class="fragment"  -->


---

#### Instruksi / User Prompt

berisi instruksi yang spesifik terhadap tugas yang harus dilaksanakan oleh LLM.

instruksi ini harus mempunyai isi yang bagus seperti contoh yang ada di basic prompting  <!-- element class="fragment"  -->

mulai dari visi besar atau overview nya, lalu perlahan sebutkan detil yang spesifik secara urut <!-- element class="fragment"  -->

`buatlah sebuah report tentang motor terbaik di indonesia, kategorikan berdasarkan harga, mulai dari entry level, mid level, dan high end. masing-masing kategori, berikan minimal 2 rekomendasi, dan sebutkan kelebihan dan kelemahannya` <!-- element class="fragment"  -->

---
#### Input Data

input data berisi data yang akan diolah oleh instruksi yang sudah kita tulis.

data ini biasanya berasal dari kita sendiri <!-- element class="fragment"  -->

masih dengan contoh mencari motor diatas, kita bisa tambahkan brosur yang kita dapatkan dari sales, sebagai referensi utama.<!-- element class="fragment"  -->

mungkin di prompt bisa ditambahkan: <!-- element class="fragment"  -->

`prioritaskan motor yang ada di dalam brosur yang di attachment`<!-- element class="fragment"  -->

---

![[https://i0.wp.com/www.hondamotorpasuruan.com/wp-content/uploads/2025/05/Brosur-Promo-Kredit-Harga-Motor-Honda-Pasuruan.webp?fit=1080%2C1343&ssl=1]]


---

#### Konteks Eksternal

berisi data tambahan yang sifatnya eksternal (bukan dari kita) yang dapat digunakan sebagai referensi hasil dari report

data eksternal ini bentuk datanya bermacam-macam, teks, audio, gambar, atau website/url<!-- element class="fragment"  -->

masih dengan contoh mencari motor diatas, kita bisa tambahkan :  <!-- element class="fragment"  -->

`check "olx.co.id", "planetmoto.com" dan "facebook.com" untuk mencari harga jual motor bekas yang paling bagus` <!-- element class="fragment"  -->

`check tokopedia dan shopee untuk mendapatkan harga motor yang terbaru` <!-- element class="fragment"  -->

---
#### Output Indicator

adalah sebuah informasi tentang format output dari LLM, atau ekspektasi kita terhadap hasil jawaban dari LLM.

tujuannya adalah untuk memberikan penekanan tentang hasil yang benar <!-- element class="fragment"  -->

masih dengan contoh mencari motor diatas, kita bisa tambahkan :  <!-- element class="fragment"  -->

`kumpulkan semua data dan buatlah sebuah tabel untuk mengelompokkan hasil report` <!-- element class="fragment"  -->
 
---

#### Hasil Akhir

`buatlah sebuah report tentang motor terbaik di indonesia, kategorikan berdasarkan harga, mulai dari entry level, mid level, dan high end. masing-masing kategori, berikan minimal 2 rekomendasi, dan sebutkan kelebihan dan kelemahannya` 
<!-- element class="fragment" style="color:lightblue"  -->

`prioritaskan motor yang ada di dalam brosur yang di attachment`<!-- element class="fragment" style="color:yellow"  -->

`check tokopedia dan shopee untuk mendapatkan harga motor yang terbaru`<!-- element class="fragment" style="color:orange"   -->

`kumpulkan semua data dan buatlah sebuah tabel untuk mengelompokkan hasil report`<!-- element class="fragment"  style="color:lightgreen"   -->

---