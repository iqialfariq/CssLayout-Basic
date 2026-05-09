# 🧠 Penjelasan CSS Layouting
<p align="justify">
CSS Layouting (tata letak CSS) adalah teknik mengatur posisi, ukuran, dan struktur elemen HTML pada halaman web menggunakan properti CSS agar tampil menarik dan terorganisir. Ini memisahkan konten (HTML) dari tampilan visualnya, memungkinkan pembuatan kerangka website modern yang **kompleks, responsif, dan fleksibel**. </p>

---
# 📌 Property dan Value CSS Layouting

## 📐 Dimensi

  <p align="justify">
  Merujuk pada properti yang digunakan untuk mengatur ukuran elemen di halaman web. Dimensi menentukan lebar, tinggi, serta batas maksimal/minimal dari sebuah elemen sehingga layout lebih terkontrol dan responsif.</p> 
  Dimensi dibagi menjadi 6 yaitu:  

  1. **Width**📎  
     Menentukan lebar elemen. Bisa berupa nilai absolut atau relatif.  
     ```html
     <div style="width: 200px; background: lightblue;">
       Elemen dengan lebar 200px
     </div>
     ```

  2. **Height**📎  
     Menentukan tinggi elemen. Sama seperti width, bisa absolut atau relatif.  
     ```html
     <div style="height: 100px; background: lightgreen;">
       Elemen dengan tinggi 100px
     </div>
     ```

  3. **Min-Width**📎  
     Menentukan lebar minimum elemen agar tidak mengecil terlalu kecil.  
     ```html
     <div style="min-width: 150px; background: pink;">
       Elemen dengan min-width 150px
     </div>
     ```

  4. **Max-Width**📎  
     Menentukan lebar maksimum elemen agar tidak melebar berlebihan.  
     ```html
     <div style="max-width: 300px; background: orange;">
       Elemen dengan max-width 300px
     </div>
     ```

  5. **Min-Height**📎  
     Menentukan tinggi minimum elemen.  
     ```html
     <div style="min-height: 80px; background: violet;">
       Elemen dengan min-height 80px
     </div>
     ```

  6. **Max-Height**📎  
     Menentukan tinggi maksimum elemen.  
     ```html
     <div style="max-height: 150px; background: yellow;">
       Elemen dengan max-height 150px
     </div>
     ```
     
---
## 📦 Box Model    
Box Model merujuk pada konsep dasar dalam web design yang menjelaskan bagaimana setiap elemen HTML diperlakukan sebagai sebuah kotak. Kotak ini terdiri dari:
- **Content** → isi utama elemen (teks/gambar).
- **Padding** → ruang antara content dan border.
- **Border** → garis pembatas di sekitar elemen.
- **Margin** → ruang kosong di luar elemen, memisahkan elemen dengan elemen lain.

## Property: Margin📎

**Margin** digunakan untuk memberikan ruang kosong di luar elemen, yaitu jarak antara elemen tersebut dengan elemen lain di sekitarnya.  
Margin bisa bernilai positif maupun negatif (`-`).

### Value Margin
Margin memiliki 4 sisi:
1. **Top**  
2. **Right**  
3. **Bottom**  
4. **Left**

### Shorthand Margin
Penulisan shorthand mengikuti urutan: **top → right → bottom → left**

```css
/* Semua sisi sama */
margin: 10px;

/* Atas-bawah | Kiri-kanan */
margin: 10px 20px;

/* Atas | Kiri-kanan | Bawah */
margin: 10px 20px 30px;

/* Atas | Kanan | Bawah | Kiri */
margin: 10px 20px 30px 40px;
```
---
## Property: Border📎
Digunakan untuk mempertegas batas sekeliling elemen, membuat kotak terlihat jelas,  
atau memberi efek dekoratif. Border memiliki beberapa gaya di antaranya:  
`solid`, `dashed`, `dotted`, `double`.

### Value Border
Border memiliki 4 sisi:
1. Top  
2. Right  
3. Bottom  
4. Left  

### Cara Menggunakan (Shorthand Border)

```css
/* Semua sisi sama */
border: 2px solid black;

/* Atas-bawah | Kiri-kanan */
border: 2px solid red 4px dashed blue;

/* Atas | Kiri-kanan | Bawah */
border: 2px solid green 4px dotted orange 6px double purple;

/* Atas | Kanan | Bawah | Kiri */
border: 1px solid red 2px dashed blue 3px dotted green 4px double black;

```
---
## Property: Padding📎
Digunakan untuk memberikan ruang kosong di dalam elemen, yaitu jarak antara **konten** dengan **border**.  
Berbeda dengan margin, padding **tidak bisa bernilai negatif (-)**.

### Value Padding
Padding memiliki 4 sisi:
1. Top  
2. Right  
3. Bottom  
4. Left

### Cara Menggunakan (Shorthand Padding)

```css
/* Semua sisi sama */
padding: 10px;

/* Atas-bawah | Kiri-kanan */
padding: 10px 20px;

/* Atas | Kiri-kanan | Bawah */
padding: 10px 20px 30px;

/* Atas | Kanan | Bawah | Kiri */
padding: 10px 20px 30px 40px;

```
---
## 🧩 Property: Box-Sizing
<p align="justify">
Merujuk pada cara browser menghitung ukuran total elemen (`width` dan `height`). Properti ini mempengaruhi apakah **padding** dan **border** ikut dihitung dalam ukuran elemen atau tidak. </p>

### Value Box-Sizing
Ada 3 value utama:

1. **content-box**  
   Default. `width` dan `height` hanya menghitung **content**. Padding dan border ditambahkan di luar ukuran elemen.  

2. **border-box**  
   `width` dan `height` menghitung **content + padding + border**. Lebih mudah untuk layout modern karena ukuran total elemen tetap konsisten.  

3. **inherit**  
   Elemen mewarisi nilai `box-sizing` dari parent‑nya.  

### Cara Menggunakan

```css
/* Default */
box-sizing: content-box;

/* Lebih praktis untuk layout */
box-sizing: border-box;

/* Mewarisi dari parent */
box-sizing: inherit;
```
---
## 🔄 CSS Reset
<p align="justify">
CSS Reset adalah kumpulan aturan CSS yang digunakan untuk menghapus atau menormalkan gaya default bawaan browser, sehingga tampilan website menjadi konsisten di semua browser. </p>

### Eric Meyer’s Reset (Klasik)📎
```css
/* Eric Meyer’s Reset CSS v2.0 (2011) */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header, hgroup,
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}

/* HTML5 display-role reset untuk browser lama */
article, aside, details, figcaption, figure,
footer, header, hgroup, menu, nav, section {
  display: block;
}

body {
  line-height: 1;
}

ol, ul {
  list-style: none;
}

blockquote, q {
  quotes: none;
}

blockquote:before, blockquote:after,
q:before, q:after {
  content: '';
  content: none;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}
```
---
## 🌊 Float
<p align="justify">
Merujuk pada cara untuk membuat elemen “ melayang ” ke kiri atau kanan dari kontainernya, memungkinkan teks atau elemen lain mengalir di sekitarnya. Sering dipakai untuk layout gambar di samping teks, atau membuat kolom sederhana sebelum era Flexbox dan Grid. </p>

### Value Float
1. **none** → elemen tidak melayang, posisi default.  
2. **left** → elemen melayang ke kiri container.  
3. **right** → elemen melayang ke kanan container.  

### Cara Menggunakan
```css
/* Elemen melayang ke kiri */
float: left;

/* Elemen melayang ke kanan */
float: right;

/* Default, tidak melayang */
float: none;
```
---
## 🧹 Clear
<p align="justify">
Merujuk pada cara untuk mengatur apakah elemen harus menghindari elemen lain yang menggunakan **float**. Ini penting untuk menjaga alur layout agar tidak tumpang tindih atau berantakan setelah elemen melayang. </p>

### Value Clear
1. **both** → elemen tidak boleh berada di samping elemen yang di-*float* kiri maupun kanan.  
2. **left** → elemen tidak boleh berada di samping elemen yang di-*float* kiri.  
3. **right** → elemen tidak boleh berada di samping elemen yang di-*float* kanan.

### Cara Menggunakan
```css
/* Elemen turun ke bawah, tidak berdampingan dengan float kiri */
clear: left;

/* Elemen turun ke bawah, tidak berdampingan dengan float kanan */
clear: right;

/* Elemen turun ke bawah, tidak berdampingan dengan float kiri maupun kanan */
clear: both;

/* nicolasgallagher */📎
.cf:before,
.cf:after {
    content: " "; /* 1 */
    display: table; /* 2 */
}

.cf:after {
    clear: both;
}
```
---
## 📍 Position
<p align="justify">
Merujuk pada cara sebuah elemen ditempatkan dalam halaman web. Properti ini bekerja bersama dengan `top`, `right`, `bottom`, dan `left` untuk mengatur posisi elemen relatif terhadap kontainer atau viewport. </p>

### Value Position
1. **static**  
   Elemen mengikuti alur normal dokumen. Tidak bisa digeser dengan `top/right/bottom/left`.

2. **relative**  
   Elemen tetap di alur normal, tapi bisa digeser relatif terhadap posisi aslinya.

3. **absolute**  
   Elemen keluar dari alur normal, diposisikan relatif terhadap ancestor terdekat yang punya posisi selain `static`.

4. **fixed**  
   Elemen diposisikan relatif terhadap viewport. Tidak bergerak saat halaman di-*scroll*.

5. **sticky**  
   Kombinasi relative + fixed. Elemen mengikuti alur normal, tapi akan “menempel” ke posisi tertentu saat di-*scroll*.

### Cara Menggunakan
```css
/* Static */
position: static;

/* Relative */
position: relative;
top: 10px;
left: 20px;

/* Absolute */
position: absolute;
top: 50px;
right: 30px;

/* Fixed */
position: fixed;
bottom: 0;
right: 0;

/* Sticky */
position: sticky;
top: 0;
```
---
## 🗂️ Z-Index
<p align="justify">
Merujuk pada cara mengatur tumpukan atau lapisan sebuah elemen HTML. Dengan `z-index`, kita bisa menentukan apakah elemen berada di paling depan atau paling belakang dibanding elemen lain. </p>

### Value Z-Index
1. **Nilai positif (1 sampai 900)** → elemen berada di atas elemen lain dengan nilai lebih rendah.  
2. **Nilai negatif (-1 sampai -900)** → elemen berada di bawah elemen lain dengan nilai lebih tinggi.

### Cara Menggunakan
```css
/* Default (auto) */
position: relative;
z-index: auto;

/* Elemen di atas */
position: relative;
z-index: 10;

/* Elemen di bawah */
position: relative;
z-index: -1;
