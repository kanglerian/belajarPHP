# Memulai Kelas

Selamat datang di kelas Belajar PHP. Disini kita akan belajar PHP Basic, sampai kita bisa membuat Website sederhana menggunakan bahasa PHP 😄
Website ini adalah dokumentasi dari hasil belajar dari berbagai sumber mengenai PHP, jadi untuk beberapa kesalahan mohon dimaafkan dan boleh dikoreksi, oke?

Let's Started! 😄

<hr>

# Introduction

## Kenapa PHP?

1. **PHP Relatif mudah untuk pemula** <br>
   ketika kita menulis beberapa baris code saja, kita sudah bisa melihat hasilnya di website. Atau contohnya, kita lihat bahasa pemrograman Java dan PHP lihat perbandingannya ketika kita ingin mencetak
   teks `Hello World`

   ```Java
   class HelloWorld{
       public static void main( String args[] ) {
           System.out.println("Hello World");
       }
   }
   ```

   ```PHP
   <?php
      echo "Hello World!";
   ?>
   ```

2. **Pre-requisite HTML + CSS**
3. **Gratis & Open Source**<br>
   Kita cukup mengunjungi websitenya untuk menginstall PHP di [https://www.php.net/downloads.php](https://www.php.net/downloads.php)
4. **Dukungan komunitas yang banyak**<br>
   Ketika searching di google atau stackoverflow di dalamnya banyak artikel dan pertanyaan yang membahas tentang PHP dan mudah untuk mencari solusi dari masalah. Termasuk ada grup facebook PHP Indonesia.
5. **Dokumentasi yang lengkap**<br>
   Diwebsite resminya saja, dokumentasinya sangat lengkap [https://www.php.net/downloads.php](https://www.php.net/downloads.php)
6. **PHP dibuat khusus untuk Web**<br>
   Diciptakan untuk membuat website, karena ada beberapa bahasa pemrograman seperti Java yang awalnya hanya dibuat untuk Desktop tapi sekarang bisa dibuat untuk Website.
7. **Kebanyakan website yang ada di Internet dibuat oleh PHP**
8. **Banyak website besar yang dibuat dengan PHP (pada awalnya)**<br>
   facebook, Yahoo, Wikipedia dan Flickr
9. **Banyak CMS (Content Management System) yang dibuat dengan PHP**<br>
   Wordpress, Joomla, Drupal atau Moodle.
10. **Banyak sekali Framework untuk PHP**<br>
    CodeIgniter, Laravel, CakePHP, Symfony, yiiframework

<hr>

## Apa yang akan kita pelajari?

1. **Memahami Client-Side vs Server-Side Scripting**<br>
   Saat kita mempelajari HTML dan CSS itu disebut Client-Side Scripting. Nah untuk PHP dia adalah Server-Side Scripting.
2. **Static & Dynamic Website**
3. **Persiapan lingkungan pengembangan**
4. **Sintaks PHP**<br>
   Penulisan bahasa PHP kita akan pelajari disini.
5. **Array**
6. **Request Method**<br>
   Metode pengiriman dan penerimaan data antar halaman.
7. **Studi kasus website sederhana**<br>
   - database
   - CRUD (Create, Read, Update, Delete)
   - login & registration
   - session & cookie (supaya login lebih secure)
   - ajax (menambah interaktivitas website)
   - upload file
   - reporting
   - web hosting

<hr>

## Apa yang harus disiapkan?

1. **Code Editor** <br>
   Kita akan pakai `Visual Studio Code`, jika teman-teman ingin menggunakan Sublime Text, Atom, Notepad ++ dan lain lain, silahkan.
2. **Web Server** <br>
   Kita akan gunakan `Apache`.
3. **Web Browser** <br>
   Kita akan pakai `Google Chrome`
4. **Database Server** <br>
   Kita akan pakai `MySQL`

<hr>

# Sejarah PHP

PHP dibuat oleh pak Rasmus Lerdorf. Pada awalnya dia membuat sebuah program dalam bahasa C untuk mengeloma Personal Page. PHP itu awalnya singkatan dari Personal Home Page. Dia bikin web form untuk terhubung ke dalam database.

- PHP/FI, 1994<br>
  Personal Home Page/Form Interpreter
- PHP Tools v.1, 1995
- PHP Tools v.2, 1997
- PHP 3, 1998<br>
  Zeev Suraski & Andi Gutmans membantu untuk mengembangkan PHP<br>
  Zend Technologies<br>
  _PHP: Hypertext Preprocessor_
- PHP 4, 2000<br>
  Zend Engine
- PHP 5, 2004<br>
  Zend Engine 2, di dalamnya sudah bisa menggunakan Object Oriented Programming (OOP)<br>
  PHP Data Object (PDO) bisa mengelola berbagai macam Database.
- PHP 5, 2004<br>
  Zend Engine 2, di dalamnya sudah bisa menggunakan Object Oriented Programming (OOP)
- PHP 6
- PHP 7, 2014<br>

<hr>

# Karakteristik Bahasa PHP

1. Ekstensi file .php
2. Ditulis di dalam tag php `<?php?>`
   - delimiter
   - diawali dengan `<?php`
   - diakhiri dengan `?>`
3. PHP bisa digunakan bersamaan dengan HTML
4. Mengikuti bahasa C

<hr>

# Apa itu Client-Side & Server-Side Scripting?

## Client-Side Scripting

Ketika kita membuat website dengan HTML, CSS dan JavaScript itu disebutnya Client-Side Scripting. Karena semua pemrosesannya ada di sisi Client. <br>

![Client Side](/images/client-side.png)

## Server-Side Scripting

![Server Side](/images/server-side.png)

<hr>

# Persiapan Lingkungan Pengembangan

- **Apache**<br>
  [https://httpd.apache.org/download.cgi](https://httpd.apache.org/download.cgi)
- **PHP**<br>
  [https://www.php.net/downloads.php](https://www.php.net/downloads.php)
- **MySQL**<br>
  [https://dev.mysql.com/downloads/](https://dev.mysql.com/downloads/)
- **All-In-One Packages**<br>
  [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html)

  <hr>

# Sintax PHP
