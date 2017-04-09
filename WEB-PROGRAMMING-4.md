# CRUD (Create, Read, Update, Delete) dengan PHP dan mySql

### Cara kerja web

![web-skema](assets/webskema.png)

### mySql

- Buka phpmyadmin

- Buat database baru (beri nama misal: “blog”)

- Buat tabel posts berisi kolom masing-masing bernama:

   - postId (type: INT, length/value: 11, A_I: cek)

   - postTitle (type: VARCHAR, length: 200)

   - postDate (type: DATETIME)

   - postContent (type: TEXT)

   - postTag (type: VARCHAR, length: 100)

   - status (type: VARCHAR, length: 10)

Atau gunakan SQL Query berikut:
```SQL
CREATE TABLE IF NOT EXISTS 'posts' (
'postId' int(11) NOT NULL AUTO_INCREMENT,
'postTitle' varchar(200) NOT NULL,
'postDate' datetime DEFAULT NULL,
'postContent' text NOT NULL,
'postTag' varchar(100) NOT NULL,
'status' varchar(10) NOT NULL,
PRIMARY KEY ('postId')
) ENGINE=InnoDB DEFAULT CHARSET=latin1 AUTO_INCREMENT=11 ;
```
![create-table](assets/query-create-table.png)
klik go

### Persiapan

- dengan browser, buka akun github [wkwksama](https://github.com/wkwksama/belajar-php-pdo)
- buka terminal
- masukkan `cd /var/www/html` terus enter
- masukkan `sudo git clone [REPO GITHUB MILIKMU]`
- info: tadi menggunakan sudo karena memerlukan akses root di directory tersebut
- karena directory web server di linux memerlukan akses root, kita perlu melakukan beberapa perubahan
   - `sudo chmod -R 775 /var/www/html/belajar-php-pdo`
   - info: perintah ini digunakan untuk membuka hak akses directory agar bisa diedit tanpa perlu root
- buka link localhost/belajar-php-pdo

Selanjutnya buka project yang kita unduh tadi dengan teks editor (atom)

- Buat file connectDB.php
- Buat file addPost.php
- Buat file publishPost.php
- Buat file editPost.php
- Buat file deletePost.php

### Koneksi dengan PDO

- tulis kode ini di file connectDB untuk membuat koneksi database

```php
<?php

$host = 'localhost';
$username = 'root';
$password = 'root';
$database = 'nama_database';
$dbms = 'mysql';
$charset = 'utf8';
$db = null;
try {
$db = new PDO("$dbms:host=$host;dbname=$database;charset=$charset", $username, $password);
$db->setAttribute(PDO::ATTR_ERRMODE, PDO::ERRMODE_EXCEPTION);
echo “koneksi berhasil”;
}
catch(PDOException $e) {
echo 'koneksi error :'.$e->getMessage();
}

?>
```
- Pada index.php setelah tag body (<body>) ketikkan kode berikut:
```php
<?php
include_once 'connecDB.php';
?>
```
- Halaman akan menampilkan pesan “koneksi berhasil” pada atas halaman.
- Jika terjadi error periksalah penulisan kode anda, seperti penulisan nama database, password, sintaks error dll.

### Create
