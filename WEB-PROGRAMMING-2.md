## Review Materi Pertemuan Kedua Doscom University

# Dasar CLI (Commad Line Interface) dan Git

## Perintah Dasar Linux
Untuk berselancar di Linux selain menggunakan Graphical User Interface(GUI) anda juga dapat menggunakan terminal. Untuk membuka terminal dapat dilihat di whisker, atau ketik `CTRL + ALT + T`, atau pada tealinux bisa dengan `F12` untuk menggunakan dropdown terminal.
Ada beberapa perintah dasar dalam terminal, yang paling banyak digunakan yaitu :
- Melihat file dan folder di direktori
  ```bash
  $ ls
  ```
- Berpindah direktori
  ```bash
  $ cd <nama folder>
  ```
- Berpindah ke direktori satu level di atasnya
  ```bash
  $ cd ..
  ```
- Membuat empty file
  ```bash
  $ touch <nama file>
  ```

## Menggunakan Git
Git merupakan version control system. Deksripsi dan cara menggunakan dapat dilihat di https://git-scm.com/
Ada beberapa perintah dasar git dalam terminal, yang paling banyak digunakan yaitu :
- Mengisi identitas git di perangkat anda
  ```bash
  $ git config --global user.name "usernameanda"
  $ git config --global user.email "emailanda@emailanda.com"
  ```
- Menginisialisasi git pada project
  ```bash
  $ git init
  ```
- Menambah record git
  ```bash
  $ git add <nama file> ///menambah file tertentu
  $ git add . ///menambah semua filenyae
  ```
- Mengcommit git
  ```bash
  $ git commit -m "pesan anda"
  ```
- Melihat log atau daftar commit
  ```bash
    $ git log
  ```
- Kembali pada commit sebelumnya
  ```bash
    $ git checkout <commit yang ingin dituju>
  ```


# Github

## Hosting Project ke Github
- Registrasi project kita ke github
  ```bash
  $ git remote add <nama inisial> <nama branch> <link git>
  ```
  Contoh :
  ```bash
  $ git remote add github master https://github.com/DOSCOM/doscom-university-2017.git
  ```
  Untuk nama git dapat anda lihat di repository github anda pada bagian `Clone or download`
- Hosting git
  ```bash
  $ git push <nama inisial> <nama branch>
  ```
  Contoh :
  ```bash
  $ git remote add github master https://github.com/DOSCOM/doscom-university-2017.git
  ```

## Menggunakan Bootstrap
Bootstrap merupakan CSS Framework. Untuk dapat menggunakan bootstrap dapat anda lihat di http://getbootstrap.com.
Untuk memasang bootstrap pada project ikuti langkah berikut
- Download bootstrap di http://getbootstrap.com/getting-started/#download
- Ekstrak archive yang telah selesai di download lalu copy ke project anda.
- Import bootstrap.min.css ke html anda

---

---
## Referensi dan Tambahan
- :bulb: [Basic git dan github oleh hacktiv8](https://github.com/hacktiv8/phase-0-activities/blob/master/modules/git-github-basics.md)
- :bulb: [Tutorial interaktif Git oleh codesaya.com](https://codesaya.com/git/)

---

---
credits:
- [hacktiv8](https://github.com/hacktiv8/)
- [codesaya.com](https://codesaya.com/git/)
- [doscom](http://doscom.org/)
