Nama   : Navyta Budi Yulia 

NIM    : 312410184

Kelas  : TI.24.A2

# Lab7Web

# Langkah dan Penjelasan

## Langkah 1
- Buat folder lab7_php_dasar di dalam direktori htdocs.
- Folder htdocs adalah tempat semua file web disimpan di XAMPP.
- Semua file .php kamu akan disimpan di sini dan diakses lewat http://localhost/lab7_php_dasar/.

<img width="1920" height="945" alt="Image" src="https://github.com/user-attachments/assets/4361f512-5b1f-4f41-b010-533161e04879" />


## Langkah 2
- Buat file `php_dasar.php` lalu tuliskan kode berikut:

```php
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>PHP Dasar</title>
</head>
<body>
  <h1>Belajar PHP Dasar</h1>
  <?php
    echo "Hello World";
  ?>
</body>
</html>
```

<img width="1920" height="942" alt="Image" src="https://github.com/user-attachments/assets/2f81e759-bdaf-46a0-8451-a9df3cb992d2" />

Penjelasan Perubahan :
  - Ini membuktikan bahwa server PHP sudah berjalan.
  - <?php ... ?> adalah blok kode PHP.
  - echo "Hello World"; menampilkan teks ke layar.

## Langkah 3
- Menambahkan Variabel

```php
  <?php
$nim = "312410184";
$nama = "Navyta Budi Yulia";
echo "NIM : $nim <br>";
echo "Nama : $nama";
?>
```

<img width="1920" height="942" alt="Image" src="https://github.com/user-attachments/assets/8f94050d-60d5-4083-bba1-995b3e4bba23" />

Penjelasan Perubahan :
  - `$nim` dan `$nama` menyimpan data (variabel PHP selalu diawali $).
  - Operator `.` digunakan untuk menggabungkan teks.
  - `<br>` untuk membuat baris baru di HTML.

## Langkah 4
- Code ditambah dengan : 

```php
<?php
echo "Selamat Datang " . $_GET['nama'];
?>
```
<img width="1920" height="942" alt="Image" src="https://github.com/user-attachments/assets/0815ace7-9686-424c-94ad-fcf5bc36ca23" />

Penjelasan perubahan :
  - Jika kamu buka http://localhost/lab7_php_dasar/php_dasar.php?nama=Navyta, maka hasilnya akan        seperti gambar di atas.
  - `$_GET` mengambil data dari URL.
 
## Langkah 5
- Membuat Form Input

```php
<form method="post">
  <label>Nama: </label>
  <input type="text" name="nama">
  <input type="submit" value="Kirim">
</form>

<?php
echo "Selamat Datang " . $_POST['nama'];
?>
```

<img width="1920" height="934" alt="Image" src="https://github.com/user-attachments/assets/ce2a2757-e676-4476-84a4-469744550f8f" />


<img width="1920" height="945" alt="Image" src="https://github.com/user-attachments/assets/afc0b92a-3de5-4d7d-85bc-893909670b45" />


<img width="1920" height="949" alt="Image" src="https://github.com/user-attachments/assets/da9521f5-b761-46d8-842d-727294c96ca6" />

Penjelasan Perubahan :
  - `method="post"` digunakan untuk mengirim data ke server secara aman.
  - Data yang dikirim ditangkap menggunakan `$_POST['nama']`.
  - Setelah tombol “Kirim” ditekan, nama akan muncul di bawah form.

## Langkah 6
- Operator dan Perhitungan

```php
<?php
$gaji = 1000000;
$pajak = 0.1;
$thp = $gaji - ($gaji * $pajak);
echo "Gaji sebelum pajak = Rp. $gaji <br>";
echo "Gaji yang dibawa pulang = Rp. $thp";
?>
```

<img width="1920" height="942" alt="Image" src="https://github.com/user-attachments/assets/d0c92165-05bd-4b2f-ace1-b2e98c5a65a4" />

Penjelasan Perubahan :
  - Menampilkan hasil perhitungan dalam format teks.
  - Operator `*` dan `-` digunakan untuk perhitungan matematika.

# Pertanyaan dan Tugas
  Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir. Dan pilihan  
  pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.
