# Lab3Web — Praktikum 3: CSS Dasar

Repository ini berisi hasil Praktikum 3 CSS Dasar.

## Tujuan Praktikum

1. Memahami konsep dasar CSS.
2. Memahami aturan penulisan CSS.
3. Memahami selector sebagai pengontrol CSS.
4. Membuat pengaturan CSS pada HTML.

## Struktur Folder

```text
Lab3Web/
├── lab2_css_dasar.html
├── lab2_css_eksternal.html
├── style_eksternal.css
└── README.md
```

## Urutan Pengerjaan

### 1. Membuat Dokumen HTML

File `lab2_css_dasar.html` berisi struktur dasar HTML, header, navigasi, bagian intro, dan tombol.

**Screenshot:**  
Tambahkan screenshot hasil tahap HTML awal di sini.

### 2. Mendeklarasikan CSS Internal

CSS internal diletakkan di dalam tag `<style>` pada bagian `<head>`.
CSS mengatur font body, header, dan heading.

**Screenshot:**  
Tambahkan screenshot hasil CSS internal di sini.

### 3. Menambahkan Inline CSS

Inline CSS diterapkan langsung pada tag `<p>` menggunakan atribut `style`.

**Screenshot:**  
Tambahkan screenshot hasil Inline CSS di sini.

### 4. Membuat CSS Eksternal

File `style_eksternal.css` dibuat terpisah dari HTML dan dihubungkan menggunakan tag `<link>`.

**Screenshot:**  
Tambahkan screenshot hasil CSS eksternal di sini.

### 5. Menambahkan CSS Selector

CSS eksternal menggunakan:
- Element selector untuk `nav` dan `nav a`
- ID selector untuk `#intro` dan `#intro h1`
- Class selector untuk `.button` dan `.btn-primary`
- Pseudo-class `:hover` pada navigasi

**Screenshot:**  
Tambahkan screenshot hasil CSS Selector di sini.

## Pertanyaan dan Tugas

### 1. Eksperimen Properti CSS

Lakukan perubahan atau penambahan properti dan nilai CSS menggunakan CSS Cheat Sheet dari modul.

**Hasil eksperimen:**  
Tuliskan perubahan yang dilakukan dan tambahkan screenshot di sini.

### 2. Perbedaan `h1 { ... }` dan `#intro h1 { ... }`

`h1 { ... }` digunakan untuk memberikan aturan CSS pada elemen `<h1>` yang sesuai dengan selector tersebut.

`#intro h1 { ... }` digunakan untuk memberikan aturan CSS pada elemen `<h1>` yang berada di dalam elemen yang mempunyai `id="intro"`.

### 3. CSS Internal, Eksternal, dan Inline

Jika aturan CSS internal, eksternal, dan inline diterapkan pada elemen yang sama, aturan inline memiliki prioritas lebih tinggi daripada aturan internal atau eksternal biasa, selama tidak ada aturan specificity atau `!important` yang mengubah hasilnya.

Contoh:

```html
<p style="color: red;">Belajar CSS</p>
```

```css
p {
    color: blue;
}
```

Teks akan tampil merah karena aturan inline lebih spesifik.

### 4. ID dan Class Selector

Jika sebuah elemen mempunyai ID dan class, dan kedua selector memberikan properti yang sama, selector ID memiliki specificity lebih tinggi daripada selector class.

Contoh:

```html
<p id="paragraf-1" class="text-paragraf">
    Contoh paragraf
</p>
```

```css
#paragraf-1 {
    color: red;
}

.text-paragraf {
    color: blue;
}
```

Hasilnya teks akan berwarna merah.

## Validasi CSS

Lakukan validasi CSS menggunakan W3C CSS Validator:

https://jigsaw.w3.org/css-validator/

Tambahkan screenshot hasil validasi di sini.

## Screenshot

Sesuai instruksi praktikum, setiap perubahan perlu didokumentasikan dengan screenshot. Setelah screenshot tersedia, masukkan gambar ke repository dan ubah bagian README ini menjadi referensi gambar yang sesuai.

## Commit dan Pengumpulan

Setelah semua file dan dokumentasi selesai:

1. Buat repository GitHub dengan nama `Lab3Web`.
2. Masukkan seluruh file project.
3. Commit hasil praktikum.
4. Push ke GitHub.
5. Kirim URL repository ke e-learning.
