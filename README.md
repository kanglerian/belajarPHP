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

1. Menggunakan buka dan tutup dengan tag `<?php?>` <br>

```PHP
   <?php
      echo "Hello World!";
   ?>
```

2. Standart Output menggunakan `echo, print, print_r, var_dump` <br>

```PHP [echo]
   <?php
      echo "Ini pakai echo";
      hasilnya : "Ini pakai echo"
   ?>
```

```PHP [print]
   <?php
      print "Ini pakai print";
      hasilnya : "Ini pakai print"
   ?>
```

```PHP [print_r]
   <?php
      print_r ("Lerian Febriana");
      hasilnya : "Lerian Febriana"
   ?>
   // untuk melihat isi dari array (digunakan untuk debugging)
```

```PHP [var_dump]
   <?php
      var_dump ("Hello!");
   ?>
   hasilnya : string(6) "Hello!"
   // untuk melihat isi dari variabel (digunakan untuk debugging)
```

```PHP [boolean]
   <?php
      echo true;
   ?>
   hasilnya : 1

   <?php
      echo false;
   ?>
   hasilnya : null (kosong)
```

## Penulisan PHP di dalam HTML

```HTML [PHP Inline]
   <h1>Hallo, <?php echo "Lerian Febriana"; ?></h1>
   <p><?php echo "Ini adalah paragraph, penjelasan"; ?></p>
```

## Penulisan HTML di dalam PHP

```PHP [HTML Inline]
   <?php
      echo "<h1>Hallo, ini HTML Inline></h1>";
   ?>
```

<hr>

## Variabel dan Tipe Data

> Variabel tidak boleh diawali dengan angka <br>
> Variabel boleh mengandung angka

```PHP [Variabel]
   <?php
   $nama = "Lerian Febriana";
   ?>
   <!DOCTYPE html>
   <html lang="en">

   <head>
      <meta charset="UTF-8">
      <meta http-equiv="X-UA-Compatible" content="IE=edge">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
   </head>

   <body>
      <h1>Hallo, <?= $nama; ?></h1>
   </body>

   </html>
```

```PHP [kalau pakai ""]
   <?php

   $nama = "Lerian Febriana";
   echo "Halo nama saya $nama";

   ?>
   hasil : maka hasilnya "Halo nama saya Lerian Febriana" nah itu benar
```

```PHP [kalau pakai '']
   <?php

   $nama = "Lerian Febriana";
   echo 'Halo nama saya $nama';

   ?>
   hasil : maka hasilnya "Halo nama saya $nama" nah itu jelek
```

```PHP [concatenation / penggabungan string]
   <?php

   $nama_depan = "Lerian";
   $nama_belakang = "Febriana";
   $nama_lengkap = $nama_depan . " " . $nama_belakang;

    echo "Halo nama saya $nama_lengkap";

   ?>
   hasil : maka hasilnya "Halo nama saya Lerian Febriana"
```

<hr>

## Operator

### Aritmatika

> Aritmatika operatornya : + - / \* %

```PHP [inline]
   <?php

   echo 1 + 1;

   ?>
   hasil : maka hasilnya adalah 2
```

```PHP [Variabel]
   <?php
   $x = 10;
   $y = 20;
   echo $x + $y;

   ?>
   hasil : maka hasilnya adalah 30
```

### Assignment

> Operator penugasan yaitu : =, +=, -=, \*=, /=, %=, .=

contoh:

```PHP [Assignment]
   <?php
   $x = 10;
   $y += 20;
   echo $x;

   ?>
   hasil : maka hasilnya adalah 30
   // Begitu juga dengan operator yang lainnya, tambahkan saja di depannya.
```

### Perbandingan

> Operator perbandingan : <, >, <=, >=, ==, !=

```PHP [Assignment]
   <?php

   var_dump(1 < 5);

   ?>
   hasil : maka hasilnya adalah bool(true)
```

```PHP [Assignment]
   <?php

   var_dump(6 < 5);

   ?>
   hasil : maka hasilnya adalah bool(false)
```

### Identitas

> Operator Identitas : ===, !==

```PHP
<?php
   var_dump(1 === "1");
?>
   hasil : maka hasilnya adalah false, karena tipe datanya berbeda (string)
```

### Logika

> Operator logika : && and, || or, ! not

```PHP
   $x = 10;
   var_dump($x < 20 && $x % 2 == 0);
   hasil : maka hasilnya adalah true, karena X lebih kecil dari 20 dan X jika dibagi 2 sisanya 0.
```

# Control Flow (Struktur Kendali)

alur bagaimana program kita dibaca oleh Intrepreter PHP. Normalnya dibaca dari atas ke bawah, dari kiri ke kanan. Ini kita bisa atur sendiri.

## Pengulangan

Ketika ingin mengerjakan sebuah blok program tanpa menulis ulang script. Disini kita akan belajar dengan

- **for** <br>

  ```PHP
  <?php
     for (inisialisasi, kondisi terminasi, increament/decrement)
  ?>
  ```

  note : inisialisasi menentukan variabel awal untuk pengulangan, kondisi terminasi untuk memberhentikan pengulangan, increment atau decrement agar pengulangannya bisa maju atau mundur

  ```PHP
  <?php
  for( $i = 0; $i < 5; $i++ ){
     echo "Hello World! ";
  }
  ?>
  ```

  note : maka hasilnya akan ada `Hello World!` sebanyak 5 kali secara horizontal.

- **while** <br>
  selama kondisinya true, maka lakukan yang ada di dalam bracketnya.

  ```PHP
  $i = 0;
  while( $i < 5 ){
     echo "Hello World";
  $i++;
  }
  ```

  note : jika kita lupa menambahkan increment maka akan terjadi looping forever.

- **do while** <br>
  Lakukan ini (do) selama hasilnya true (while).

  ```PHP
  $i = 0;
  do {
     echo "Hello World!";
  $i++;
  } while ($i < 5)
  ```

  hasil : maka hasilnya adalah 5 kali pengulangan `hello world` secara horizontal.

  Nah, apa perbedaannya? perbedaannya terletak ketika hasil akhirnya adalah `false`, dia tetap melakukan pengulangan 1x yang artinya jika disini maka akan mengeluarkan tek `Hello World!`.

- **foreach (digunakan untuk array)** <br>

- **Contoh sederhana Latihan 1** <br>

  ```PHP
     <table border="1" cellspacing="0" cellpadding="10">
        <?php
        for ($i = 1; $i <= 3; $i++) {
              echo "<tr>";
              for ($j = 1; $j <= 5; $j++) {
                 echo "<td>$i,$j</td>";
              }
              echo "</tr>";
        }
        ?>
     </table>
  ```

  ![ImagePHP](/images/result-looping.png)

  atau <br>

  ```PHP
     <table border="1" cellspacing="0" cellpadding="10">
        <?php for($i = 1; $i <= 3; $i++) : ?>
            <tr>
               <?php for($j = 1; $j <= 5; $j++ ) : ?>
                  <td><?= "$i,$j"; ?></td>
               <?php endfor; ?>
            </tr>
        <?php endfor; ?>
     </table>
  ```

## Pengkondisian

- **if.. else** <br>

  ```PHP
   $x = 10;
   if($x < 20){
      echo "Benar";
   }else {
      echo "Salah";
   }
  ```

- **if.. elfeif.. else** <br>

  ```PHP
   $x = 30;
   if($x < 20){
      echo "Benar";
   }elseif($x == 20){
      echo "Bingo!";
   }
   else {
      echo "Salah";
   }
  ```

- ternary (menggantikan if dan else menjadi sederhana)
- switch

# Function

Potongan baris baris kode yang akan mempermudah kita dalam membuat program. Kode program ini kita bisa kasih nama dan kita panggil berulang-ulang.

## **Built in function** <br>

Date/Time : time(), date(), mktime(), strtotime()

- **Date**

```PHP Date
<?php
   echo date("l, d-M-Y");
?>
hasinya: Friday, 12-Maret-2021
```

- **Time**

```PHP Time
<?php
   // ini akan menampilkan waktu dari tanggal 1 januari 1970
   echo time();
?>
```

- **Latihan**

```PHP Time Latihan
<?php
echo date("l", time() + 172800);
?>
hasilnya: 2 hari dari hari ketika kode di eksekusi. Nilai 172800 adalah 2 hari dari sekarang berupa detik. 60 * 60 * 24 * 2
```

```PHP Time Latihan 2
<?php
echo date("d M Y", time() + 60 * 60 * 24 * 2);
?>
hasilnya: 2 hari dari sekarang
```

- **mktime** <br>
  Membuat detik sendiri dengan mktime(0,0,0,0,0,0), jam menit detik bulan tanggal tahun

  ```PHP Ulang Tahun
   <?php
   echo mktime(0,0,0,26,2,1998);
   ?>
   hasilnya: 949446000
  ```

  ```PHP Ulang Tahun Result
  <?php
  echo date("l", mktime(0,0,0,26,2,1998));
  ?>
  hasilnya: Thursday
  ```

- **strtotime** <br>

```PHP
<?php
echo strtotime("25 aug 1985");
?>
```

- **String** : **strnlen()** untuk mengukur panjang string, **strcmp()** untuk menggabungkan string, **explode()** memecah string menjadi array, contoh mengambil nama sebuah file, nama dan ekstensi. **htmlspecialchars()** menjaga dari hacker

- **Utility** : **var_dump()** mencetak array atau object, atau string pada saat debugging. **isset()** apakah sebuah variabel sudah dibuat. **empty()** apakah variabel yg ada kosong atau tidak. **die()** memberhentikan program. **sleep()** berhenti dengan waktu tertentu

## User Defined function

Kita membuat sendiri function, ketika membuat project terkadang kita harus membuat sebuah function secara manual.

- **Membuat function salam**

  ```PHP
  <?php
   function salam(){
      return "Halo selamat datang!";
   }
  ?>
  <html>
    <head>
      <title>Sapa</title>
    </head>
    <body>
      <h1><?= salam(); ?></h1>
    </body>
  </html>
  ```

  > maka hasilnya : Halo selamat datang!

- **Membuat function salam dengan parameters** <br>

  ```PHP
  <?php
     function salam($waktu = "datang", $nama = "Peserta didik baru"){
        return "Halo selamat $waktu $nama!";
     }
  ?>
  <html>
     <head>
        <title>Sapa</title>
     </head>
     <body>
        <h1><?= salam("pagi", "Lerian"); ?></h1>
     </body>
  </html>
  ```

  > maka hasilnya: Halo selamat pagi Lerian. Jika parameters tidak diisi maka akan menghasilkan Halo selamat datang Peserta didik baru.
