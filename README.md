## Property dan Value CSS Layouting

## Dimensi
  Merujuk pada properti yang digunakan untuk mengatur ukuran elemen di halaman web.  
  Dimensi menentukan lebar, tinggi, serta batas maksimal/minimal dari sebuah elemen sehingga layout lebih terkontrol dan responsif.  
  Dimensi dibagi menjadi 6 yaitu:  

  1. **Width**  
     Menentukan lebar elemen. Bisa berupa nilai absolut atau relatif.  
     ```html
     <div style="width: 200px; background: lightblue;">
       Elemen dengan lebar 200px
     </div>
     ```

  2. **Height**  
     Menentukan tinggi elemen. Sama seperti width, bisa absolut atau relatif.  
     ```html
     <div style="height: 100px; background: lightgreen;">
       Elemen dengan tinggi 100px
     </div>
     ```

  3. **Min-Width**  
     Menentukan lebar minimum elemen agar tidak mengecil terlalu kecil.  
     ```html
     <div style="min-width: 150px; background: pink;">
       Elemen dengan min-width 150px
     </div>
     ```

  4. **Max-Width**  
     Menentukan lebar maksimum elemen agar tidak melebar berlebihan.  
     ```html
     <div style="max-width: 300px; background: orange;">
       Elemen dengan max-width 300px
     </div>
     ```

  5. **Min-Height**  
     Menentukan tinggi minimum elemen.  
     ```html
     <div style="min-height: 80px; background: violet;">
       Elemen dengan min-height 80px
     </div>
     ```

  6. **Max-Height**  
     Menentukan tinggi maksimum elemen.  
     ```html
     <div style="max-height: 150px; background: yellow;">
       Elemen dengan max-height 150px
     </div>
     ```

## Box Model     
**Box Model** adalah konsep dasar dalam web design yang menjelaskan bagaimana setiap elemen HTML diperlakukan sebagai sebuah kotak. Kotak ini terdiri dari:
- **Content** → isi utama elemen (teks/gambar).
- **Padding** → ruang antara content dan border.
- **Border** → garis pembatas di sekitar elemen.
- **Margin** → ruang kosong di luar elemen, memisahkan elemen dengan elemen lain.

---

## Property: Margin

**Margin** digunakan untuk memberikan ruang kosong di luar elemen, yaitu jarak antara elemen tersebut dengan elemen lain di sekitarnya.  
Margin bisa bernilai positif maupun negatif (`-`).

### Value Margin
Margin memiliki 4 sisi:
1. **Top**  
2. **Right**  
3. **Bottom**  
4. **Left**

---

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


# 📘 Dokumentasi CSS Dasar

## 🎨 Property: Border
Digunakan untuk mempertegas batas sekeliling elemen, membuat kotak terlihat jelas,  
atau memberi efek dekoratif. Border memiliki beberapa gaya di antaranya:  
`solid`, `dashed`, `dotted`, `double`.

---

### 💡 Value Border
Border memiliki 4 sisi:
1. Top  
2. Right  
3. Bottom  
4. Left  

---

### 🛠 Cara Menggunakan (Shorthand Border)

```css
/* Semua sisi sama */
border: 2px solid black;
