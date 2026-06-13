---
width: "1920"
---
# Pertemuan 7

---
## Teknik Prompting

Ketika kita ingin mengolah data yang jauh lebih besar lagi dan mendapatkan hasil yang sangat amat spesifik, maka kita harus naik level lagi

dengan teknik prompting ini, kita dapat memaksimalkan potensi dan fitur-fitur LLM sepenuhnya, terutama ketika LLM menghadapi pertanyaan atau permasalahan yang kompleks<!-- element class="fragment"   -->

Teknik prompting yang advanced ini berfokus kepada konteks eksternal yang diberikan ke LLM <!-- element class="fragment"   -->

---

### One Shot / Zero Shot

"Shot" adalah sebuah aksi dimana kita bertanya ke LLM, atau proses prompting secara normal.

One atau Zero shot, berarti kita "bertanya" ke LLM cuma sekali, lalu kita langsung mendapatkan jawaban akhir dari LLM <!-- element class="fragment"   -->

---

seperti kata-kata mutiara dari bang franco

![[4c0b9408848d4f8d54012703d1f79607 1.jpg]]<!-- element class="fragment"   -->

(padahal sering ga kena)<!-- element class="fragment"   -->

---
### Few Shot

Few shot, berarti kita "bertanya" ke LLM beberapa kali <!-- element class="fragment"   -->

bisa untuk memberikan informasi secara bertahap, sehingga LLM tidak langsung memproses pertanyaan pertama <!-- element class="fragment"   -->

---

![[Pasted image 20251113154806.png]]

---

Teknik ini bisa juga digunakan untuk mengedit atau menambah detil dari sebuah report 

namun biasanya LLM akan merubah bagian teks yang tidak kita ingin,<!-- element class="fragment"   -->

maka kita harus sangat spesifik dalam menentukan mana yang harus diubah <!-- element class="fragment"   -->

---

### Chain Of Thought

![[Pasted image 20251113155841.png]]


---

Chain of thought adalah proses prompting yang menggunakan langkah-langkah penalaran untuk menjawab hasil akhir

Fitur Chain of thought ini sudah tertanam di dalam model Gemini 2.5 (flash atau pro), jadi kita tidak perlu men-trigger nya secara manual <!-- element class="fragment"   -->

---
![[Pasted image 20251113160429.png]]

---
#### Tanpa Chain of Thought

prompt : `I went to the market and bought 10 apples. I gave 2 apples to the neighbor and 2 to the repairman. I then went and bought 5 more apples and ate 1. How many apples did I remain with?` <!-- element class="fragment"   -->

result: `11 apples` <!-- element class="fragment"   -->

---
#### Dengan Chain of Thought

prompt : `I went to the market and bought 10 apples. I gave 2 apples to the neighbor and 2 to the repairman. I then went and bought 5 more apples and ate 1. How many apples did I remain with?` <!-- element class="fragment"   -->

`Let's think step by step.` <!-- element class="fragment"   -->

result:  `First, you started with 10 apples.` <!-- element class="fragment"   -->
`You gave away 2 apples to the neighbor and 2 to the repairman, so you had 6 apples left.`<!-- element class="fragment"   -->
`Then you bought 5 more apples, so now you had 11 apples.` <!-- element class="fragment"   -->

`Finally, you ate 1 apple, so you would remain with 10 apples.` 
<!-- element class="fragment"   -->

---

## Agentic AI

Agentic AI adalah sebuah sistem yang mempunyai LLM sebagai "otak" nya, dan sistem ini dapat menggunakan alat (tools) dan ingatan(memory) untuk membantu menjalankan tugasnya

berikut adalah komponen dari agentic ai:


![[agent-components.webp]]

---
### Planning

Cara berpikir dari Agentic AI sedikit berbeda dari LLM biasanya.

Agentic pasti menggunakan chain of thought, namun agentic berpikir untuk mengerahkan semua yang dia punya, termasuk tools dan memory <!-- element class="fragment"   -->

---

### Tools

Tools adalah alat-alat yang dapat digunakan oleh Agentic AI.

Alat ini akan membantu Agentic AI untuk menyelesaikan tugasnya.<!-- element class="fragment"   -->

Alat dapat berupa:
- Internet Browser <!-- element class="fragment"   -->
- Code Compiler <!-- element class="fragment"   -->
- Kalkulator <!-- element class="fragment"   -->
- Model Machine Learning lain (untuk generate image)<!-- element class="fragment"   -->
- Dan masih banyak lagi...<!-- element class="fragment"   -->

---

### Memory

ingatan atau memori dari Agentic AI mempunyai 2 tipe yang jalan secara bersamaan

#### Short Term / Working Memory <!-- element class="fragment"   -->
- berfungsi sebagai "buffer" diantara prompt few-shots <!-- element class="fragment"   -->
- dapat digunakan untuk pembelajaran konteks <!-- element class="fragment"   -->
- membantu "continuity" dan iterasi ketika proses prompting <!-- element class="fragment"   -->
#### Long Term Memory <!-- element class="fragment"   -->
- menyimpan semua histori percakapan/prompt <!-- element class="fragment"   -->
- menggunakan database vector <!-- element class="fragment"   -->


---

![[task-planner-agent.webp]]



---

### Contoh Penggunaan Agentic AI : Membuat sebuah dokumen

![[prompt-chaining.webp]]

1. sistem menerima pesan (chat message)
2. sistem membuat sebuah outline dokumen (kerangka) menggunakan gpt 4.1 mini
3. sistem mengecek hasil outline dengan kriteria yang sudah ditetapkan
4. hasil dari sistem di cek secara manual oleh manusia (set grade)
5. jika lolos pengecekan, maka kerangka akan dikembangkan menjadi dokumen penuh, menggunakan gpt-4o
6. step akhir untuk checking dan polish detil dari dokumen, juga menggunakan gpt-4o

---

https://www.youtube.com/watch?v=LAF-lACf2QY
https://www.promptingguide.ai/introduction/elements
https://learnprompting.org/docs/basics/prompt_structure
Prompt engineering

---


6. Prompting LLM
	1. tipe data
		1. text
		2. image
		3. docs
	2. Prompt Engineering
		1. Basic Prompting
		2. Prompt Elements
		3. Prompt Techniques
			1. Zero-Shot
			2. Few-Shot
			3. Chain-Of-Thought