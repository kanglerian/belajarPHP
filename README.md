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

---

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

---

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

---

# Array

Sebuah variabel yang bisa menampung lebih dari 1 nilai. Kenapa kita memerlukannya? seperti tempat pensil warna. Repot ketika kita harus mencari warna tertentu jika pensilnya tidak disimpan disebuah tempat. Jika menggunakan sebuah tempat pensil, maka akan tersimpan dengan rapih dan gampang dicari. Disini kita akan beri contoh **array numeric** yaitu array yang indexnya angka. dan **array associative** yaitu indexnya string yang kita buat untuk mengasosiasikan dengan nilainya.

```PHP cara lama
<?php
   $hari = array("Senin, Selasa, Rabu, Kamis, Jumat, Sabtu, Minggu");
?>
```

```PHP cara baru
<?php
   $bulan = ["Januari","Februari","Maret","April","Mei","Juni"];
?>
```

> Tipe data pada array boleh berbeda, contohnya element-element bisa digabung antara string, integer boolean dan lain lain.

---

## Cara menampilkan Array Debugging

- **var_dump**<br>

  ```PHP
  <?php
     $hari = ["Senin", "Selasa", "Rabu"];
     var_dump($hari);
  ?>
  ```

  hasilnya : array(3) { [0]=> string(5) "Senin" [1]=> string(6) "Selasa" [2]=> string(4) "Rabu" }

  > array pasangannya antara **key** dan **value**, key-nya adalah index yang dimulai dari 0.

- **print_r**<br>

  ```PHP
  <?php
    $hari = ["Senin", "Selasa", "Rabu"];
    print_r($hari);
  ?>
  ```

  hasilnya : Array ( [0] => Senin [1] => Selasa [2] => Rabu )

- **Menampilkan satu element** <br>
  tampilkan hari selasa. Gunakan perintah `echo` untuk menampilkannya.

  ```PHP
  <?php
     $hari = ["Senin","Selasa","Rabu"];
     echo $hari[1];
  ?>
  ```

  hasilnya: Selasa

## Menambahkan element baru pada Array

- **Tambah element di akhir**

  ```PHP
  <?php
     $hari = ["Senin","Selasa","Rabu"];
     $hari[] = "Kamis";
  ?>
  ```

  hasilnya: array(4) { [0]=> string(5) "Senin" [1]=> string(6) "Selasa" [2]=> string(4) "Rabu" [3]=> string(5) "Kamis" }

---

## Menampilkan Array (pengulangan)

- **Gunakan `for` untuk menampilkan di website.**

```PHP
<?php
$hari = ["Senin", "Selasa", "Rabu", "Kamis", "Jum'at", "Sabtu", "Minggu"]

?>

<!DOCTYPE html>
<html lang="en">

<head>
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Hari-hari</title>
<style>
   div {
         height: 50px;
         width: 70px;
         line-height: 50px;
         background-color: salmon;
         margin: 3px;
         float: left;
         text-align: center;
   }
</style>
</head>

<body>

<?php for ($i = 0; $i < count($hari); $i++) : ?>
   <div> <?= $hari[$i]; ?> </div>
<?php endfor; ?>

</body>

</html>
```

---

- **Menambahkan element pada Array** <br>
  Tambahkan `count` di `for` untuk menghitung otomatis.

```PHP
   <?php
$hari = ["Senin", "Selasa", "Rabu", "Kamis", "Jum'at", "Sabtu", "Minggu"];
$hari[] = "Libur";

?>

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hari-hari</title>
    <style>
        div {
            height: 50px;
            width: 70px;
            line-height: 50px;
            background-color: salmon;
            margin: 3px;
            float: left;
            text-align: center;
        }
    </style>
</head>

<body>

    <?php for ($i = 0; $i < count($hari); $i++) : ?>
        <div> <?= $hari[$i]; ?> </div>
    <?php endfor; ?>

</body>

</html>
```

---

- **Menggunakan `foreach` untuk menampilkan di website.**

  ```PHP
  <?php foreach ($hari as $h) : ?>
       <div><?= $h; ?></div>
   <?php endforeach; ?>
  ```

- **Latihan 1** <br>
  Menampilkan semua data secara langsung.

  ```PHP foreach
     <ul>
       <?php foreach ($mahasiswa as $mhs) : ?>
           <li><?= $mhs; ?></li>
       <?php endforeach; ?>
     </ul>
  ```

  ```PHP foreach echo
    <ul>
        <li><?= $mahasiswa[0]; ?></li>
        <li><?= $mahasiswa[1]; ?></li>
        <li><?= $mahasiswa[2]; ?></li>
        <li><?= $mahasiswa[3]; ?></li>
    </ul>
  ```

---

## Array Multidimensi

Ada Array di dalam array.

```PHP
<?php
$mahasiswa = [

 ["Lerian Febriana", "04020202", "Manajemen Informatika", "kanglerian@gmail.com"],
 ["Ummu Hanin", "03030303", "Perpajakan", "ummuhanin@gmail.com"],

];

?>
```

```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Mahasiswa</title>
</head>

<body>

    <h1>Daftar Mahasiswa</h1>
    <?php foreach ($mahasiswa as $mhs) : ?>
        <ul>
            <li><?= $mhs[0]; ?></li>
            <li><?= $mhs[1]; ?></li>
            <li><?= $mhs[2]; ?></li>
            <li><?= $mhs[3]; ?></li>
        </ul>
    <?php endforeach; ?>

</body>

</html>
```

---

```HTML
<body>

    <p>Coba cetak nama Ummu Hanin?</p>
    <h1><?= $mahasiswa[1][0]; ?></h1>

</body>
```

---

```PHP
<?php
$angka = [[1,2,3],[4,5,6],[7,8,9]];
echo $angka[1][1];
?>
```

# Associative Array

Bagaimana jika value di dalam element Array tertukar, nah ini adalah solusi dari masalah itu. Kita ngasih tau PHP bahwa contoh value ini nama lho, value ini NRP lho, value ini alamat lho. Karena yang sebelumnya itu array numeric. **Key nya itu adalah string yang kita buat sendiri**. Dan yang sekarang kita bikin sendiri :

```PHP
$mahasiswa = [
   "nama" => "Lerian Febriana",
   "nrp" => "010234023",
   "email" => "kanglerian@gmail.com",
   "jurusan" => "Sistem Informasi"
];
echo $mahasiswa["nama"];
```

> hasilnya : Lerian Febriana

```PHP Multidimensi
$mahasiswa = [

    [
        "nama" => "Lerian Febriana",
        "nrp" => "010234023",
        "email" => "kanglerian@gmail.com",
        "jurusan" => "Sistem Informasi"
    ],
    [
        "nama" => "Ummu Hanin",
        "nrp" => "0464547493",
        "email" => "umuhannin@gmail.com",
        "jurusan" => "Perpajakan"
    ],

];
echo $mahasiswa[1]["nama"];
```

> hasilnya : Ummu Hanin

```PHP Multidimensi
$mahasiswa = [

    [
        "nama" => "Lerian Febriana",
        "nrp" => "010234023",
        "email" => "kanglerian@gmail.com",
        "jurusan" => "Sistem Informasi"
    ],
    [
        "nama" => "Ummu Hanin",
        "nrp" => "0464547493",
        "email" => "umuhannin@gmail.com",
        "jurusan" => "Perpajakan",
        "tugas" => [90,80,70]
    ],

];
echo $mahasiswa[1]["tugas"][0];
```

> hasilnya : 90

---

```PHP
<?php
$mahasiswa = [

    [
        "nama" => "Lerian Febriana",
        "nrp" => "04020202",
        "jurusan" => "Manajemen Informatika",
        "email" => "kanglerian@gmail.com",
        "photo" => "photo1.png"
    ],
    [
        "nama" => "Ummu Hanin",
        "nrp" => "0878862",
        "jurusan" => "Perpajakan",
        "email" => "ummuhanin@gmail.com",
        "photo" => "photo2.png"
    ],

];

?>
```

```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Mahasiswa</title>
</head>

<body>

    <h1>Daftar Mahasiswa</h1>
    <?php foreach ($mahasiswa as $mhs) : ?>
        <ul>
            <li>
                <img src="img/<?= $mhs["photo"] ?>" alt="">
            </li>
            <li>Nama: <?= $mhs["nama"]; ?></li>
            <li>NRP: <?= $mhs["nrp"]; ?></li>
            <li>Jurusan: <?= $mhs["jurusan"]; ?></li>
            <li>Email: <?= $mhs["email"]; ?></li>
        </ul>
    <?php endforeach; ?>

</body>

</html>
```

# GET & POST

## Variabel Scope

```PHP
<?php

$x = 10;

function tampilX(){
   $x = 20;
   echo $x;
}

tampilX();
echo "<br>";
echo $x;

?>

```

> Maka hasilnya adalah : 20 dan 10. Kenapa berbeda? karena yang ada difunction dia punya lingkup sendiri. Kalau $x = 10; itu variabel lokal khusus file ini.

```PHP
<?php

$x = 10;

function tampilX(){
   global $x;
   echo $x;
}

tampilX();
echo "<br>";
echo $x;

?>

```

> Maka hasilnya adalah : 10. Karena global akan mencari "ada tidak variabel X di luar function?"

---

## Super Globals

adalah variabel-variabel yang sudah dimiliki oleh PHP yang bisa kita gunakan dimanapun dan kapanpun di dalam halaman PHP kita. Dan semua ini adalah **array assosiative**.

- **$\_GET**<br>
  ```PHP
  <?php
     var_dump($_GET);
  ?>
  ```
  > hasilnya : array(0) { }
- **$\_POST**<br>

```PHP
  <?php
     var_dump($_POST);
  ?>
```

> hasilnya : array(0) { }

---

Cara untuk memasukan data ke $\_GET maka tinggal tulis seperti ini :

```PHP
<?php
   $_GET["nama"] = "Lerian Febriana";
   $_GET["nrp"] = "1100293739";

   var_dump($_GET);
?>
```

---

Atau kita bisa menulisnya di url address browser kita, dengan menambahkan `?` untuk memasukan data ke dalam $\_GET seperti ini :

`http://localhost/belajarPHP/index.php?nama=Lerian%20Febriana` <br>

> hasilnya : array(1) { ["nama"]=> string(15) "Lerian Febriana" } <br>

Menambahkan data variabel lagi dengan menambahkan `&` seperti ini : <br>

`http://localhost/belajarPHP/index.php?nama=Lerian%20Febriana&nrp=124863511` <br>

> hasilnya : array(1) { ["nama"]=> string(15) "Lerian Febriana" ["nrp"]=> string(9) "124863511" } <br>

---

- **$\_SERVER**<br>

```PHP
  <?php
     var_dump($_SERVER);
  ?>
```

> hasilnya : informasi server kita.

```PHP
<?php
   echo $_SERVER["SCRIPT_FILENAME"];
?>
```

> hasilnya: /opt/lampp/htdocs/belajarPHP/index.php

- **$\_SESSION**<br>
- **$\_COOKIE**<br>
- **$\_REQUEST**<br>
- **$\_ENV**<br>
