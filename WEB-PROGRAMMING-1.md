# Review Materi Pertemuan Pertama Doscom University #

## Index Materi

### HTML
#### Membuat file html sederhana
Untuk membuat file html anda cukup membuat file dengan menggunakan text editor. Kemudian simpan file tersebut dengan nama yang anda kehendaki dengan ekstensi `.html`. Selamat anda sudah dapat membuat file html \(^0^)/

#### Memahami struktur HTML
HTML sendiri memiliki struktur hirarkiah sebagai berikut :
```html
<html>
  <head></head>
  <body></body>
</html>
```
Jadi untuk struktur HTML harus memiliki tag html yang didalamnya terdapat tag head dan body (baik tag pembuka dan tag penutup)

#### Menggunakan komentar HTML
Untuk memberikan komentar anda dapat menyisipkan tag `<!-- -->` berikut pada konten yang dikehendaki. Sebagai contoh :
```
  <!-- konten yang dikehendaki -->
```
atau jika anda menggunakan text editor atom anda dapat menekan `CTRL + /` pada baris yang akan anda komentar.

#### Menulis Judul menggunakan Heading
Untuk menulis judul anda dapat memilih menggunakan tag `h1`, `h2` sampai `h6`. Besar kecilnya heading mempengaruhi besar kecilnya ukuran judul. Jadi semakin besar heading semakin kecil ukuran judulnya dan sebaliknya.
Sebagai contoh :
```html
<h1>Judul dengan h1</h1>
<h2>Judul dengan h2</h2>
<h6>Judul dengan h6</h6>
```

#### Menulis kalimat atau paragraf menggunakan Paragraph
Untuk menulis kalimat anda dapat meletakkanya di dalam tag `p`. Sebagai contoh :
```html
<p>
  Ini kalimat pertama. Ini kalimat kedua. Ini kalimat ketiga. Ini kalimat keempat. Ini kalimat kelima. Ini kalimat keenam. Ini kalimat ketujuh. Ini kalimat kedelapan. Ini kalimat kesembilan. Ini kalimat kesepuluh.
</p>
```

#### Mengganti baris menggunakan Line Breaker
Untuk mengganti baris anda dapat menggunakan tag `br`. Sebagai contoh :
```html
<p>
  Ini baris pertama.<br>
  Ini baris kedua.<br>
  Ini baris ketiga.<br>
  Ini baris keempat.<br>
  Ini baris kelima.<br>
</p>
```

#### Mengelompokkan konten menggunakan Div
Dalam HTML untuk setiap konten yang ditulis biasanya dikelompokkan kedalam satu tempat di dalam tag `div`. Div ini akan mempermudah anda dalam melakukan kostumisasi tiap kontenya. Sebagi contoh :
```html
<div>
  <h1>Ini judul konten</h1>
  <p>
    Ini isi konten.
  </p>
</div>
```

#### Menambahkan gambar
Untuk Menambahkan gambar pada laman web, anda dapat menggunakan tag `img`. Tag tersebut sendiri mengharuskan kita untuk memasukkan parameter berupa letak file tersebut berada (menggunakan parameter `src`). Sebagai contoh :
```html
<img src="">
```
Berdasarkan letak filenya ada beberapa cara untuk menambahkan gambar yaitu :
- Memasukan gambar dalam direktori yang sama
  Apabila gambar anda berada di satu direktori yang sama (semisal /home/dosom/Document) anda dapat menggunakan
  ```html
  <img src="gambaranda.jpg">
  ```
- Memasukkan gambar di direktori yang berbeda
  Apabila gambar anda berada di satu direktori yang berbeda (semisal file html ada berada di /home/dosom/Document dan gambar ada berada di /home/doscom/Document/Gambar) anda dapat menggunakan
  ```html
  <img src="Gambar/gambaranda.jpg"/>
  ```
- Gambar online
  Apabila anda ingin menambahkan gambar yang berada di internet anda dapat menggunakan
  ```html
  <img src="http://www.urlanda.com/gambaranda.jpg">
  ```

#### Menggunakan Link
Untuk Menambahkan link pada laman web, anda dapat menggunakan tag `a`. Tag tersebut sendiri mengharuskan kita untuk memasukkan parameter berupa letak file tersebut berada (menggunakan parameter `href`). Sebagai contoh :
```html
<a href=""></a>
```
Berdasarkan kegunaanya ada beberapa cara untuk menggunakan link yaitu :
- Menggunakan link untuk berpindah ke posisi tertentu
  Apabila anda ingin berpindah ke posisi tertentu semisal anda berada di bagian laman paling bawah dan ingin naik ke laman paling atas. Pertama anda harus menambahkan id pada indikator yang menunjukkan bahwa dia berada di laman paling atas (bisa judul dan sebagainya). Contoh ini menggunakan judul :
  ```html
  <h1 id="PalingAtas">Ini Judul Paling Atas</h1>
  <p>
    Ini paragraf yang panjang.
  </p>
  <a href="#PalingAtas">Link ke laman paling atas</a>
  ```
- Menggunakan link untuk berpindah ke file html lain
  Untuk berpindah ke file html lain anda dapat menggunkan
  ```html
  <a href="fileHtmlYangAndaInginkan.html">Link ke laman html yang anda inginkan</a>
  ```
- Menggunakan link untuk menuju URL tertentu
  Untuk menuju URL tertentu anda dapat menggunkan
  ```html
  <a href="http://www.urlAnda.com">Link ke URL anda</a>
  ```

- Memasukan gambar dalam direktori yang sama
  Apabila gambar anda berada di satu direktori yang sama (semisal /home/dosom/Document) anda dapat menggunakan
  ```html
  <img src="gambaranda.jpg">
  ```
- Memasukkan gambar di direktori yang berbeda
  Apabila gambar anda berada di satu direktori yang berbeda (semisal file html ada berada di /home/dosom/Document dan gambar ada berada di /home/doscom/Document/Gambar) anda dapat menggunakan
  ```html
  <img src="Gambar/gambaranda.jpg"/>
  ```
- Gambar online
  Apabila anda ingin menambahkan gambar yang berada di internet anda dapat menggunakan
  ```html
  <img src="http://www.urlanda.com/gambaranda.jpg">
  ```


### CSS
#### Cara menginjek CSS ke dalam HTML
- Menggunakan tag
- Menulisnya di dalam
- Export File

### Menggunakan CSS

### Menggunakan id dan div untuk menggunakan css pada konten
