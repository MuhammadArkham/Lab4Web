# Praktikum 4 

Nama  : [Muhammad Arkhamullah Rifai Asshidiq]  
NIM   : [312410545]  
Kelas : [TI.24.A5]  
Mata Kuliah:[Pemrograman Web 1]  
Dosen Pengampu:[Agung Nugroho, S.Kom., M.Kom]  

---
## Pertanyaan

1. Tambahkan Layout untuk menu About

=> buat single layout yang berisi deskripsi, portfolio, dll

2. Tambahkan layout untuk menu Contact

=> yang berisi form isian: nama, email, message, dll

## jawaban

## 1. Halaman About

Halaman ini dibuat untuk memenuhi tugas pertama, yaitu menambahkan halaman **About** yang berisi deskripsi singkat dan portfolio.  
File yang digunakan adalah `about.html`.  
Struktur layout-nya mengikuti format yang sudah ada pada `home.html`, menggunakan elemen `<header>`, `<nav>`, `<section>`, `<aside>`, dan `<footer>`.

###  Kode HTML `about.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div id="container">
    <header>
        <h1>Tentang Kami</h1>
    </header>
    <nav>
        <a href="home.html">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html" class="active">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>

    <section id="wrapper">
        <section id="main">
            <article class="entry">
                <h2>Deskripsi</h2>
                <p>Website ini dibuat untuk mempelajari struktur layout HTML5 & CSS Float.
                   Modul ini merupakan bagian dari praktikum Pemrograman Web.</p>
            </article>

            <hr class="divider" />

            <article class="entry">
                <h2>Portfolio</h2>
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/7b8a70/fff.png" class="image-circle">
                        <h3>Project 1</h3>
                        <p>Desain layout website sederhana.</p>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" class="image-circle">
                        <h3>Project 2</h3>
                        <p>Implementasi CSS Float dan Box Model.</p>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" class="image-circle">
                        <h3>Project 3</h3>
                        <p>Membuat layout responsif dasar.</p>
                    </div>
                </div>
            </article>
        </section>

        <aside id="sidebar">
            <div class="widget-box">
                <h3 class="title">Info</h3>
                <p>Halaman ini berisi profil dan hasil proyek sederhana mahasiswa.</p>
            </div>
        </aside>
    </section>

    <footer>
        <p>&copy; 2025 - Universitas Pelita Bangsa</p>
    </footer>
</div>
</body>
</html>
 ```
Penjelasan:
```
Bagian <header> menampilkan judul halaman “Tentang Kami”.

<nav> berisi menu navigasi utama yang mengarah ke empat halaman.

<section id="main"> berisi konten utama seperti deskripsi dan portfolio.

<div class="row"> dan <div class="box"> digunakan untuk membuat tiga kolom sejajar.

Gambar diberikan class .image-circle agar berbentuk bulat.

CSS-nya tetap memakai file style.css, sehingga tampilan antarhalaman seragam.
```
Tampilan halaman About:
![gambar](https://github.com/MuhammadArkham/Lab4Web/blob/main/foto/Screenshot%202025-10-15%20191715.png?raw=true)

## 2.Halaman Kontak

Halaman Kontak dibuat untuk memenuhi tugas kedua pada praktikum.
Halaman ini berfungsi sebagai form sederhana agar pengunjung bisa mengirimkan pesan.
Form terdiri dari tiga kolom input yaitu Nama, Email, dan Pesan, serta tombol Kirim Pesan.
File ini disimpan dengan nama kontak.html.

Kode HTML – kontak.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kontak</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div id="container">
    <header>
        <h1>Kontak Kami</h1>
    </header>
    <nav>
        <a href="home.html">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html" class="active">Kontak</a>
    </nav>

    <section id="wrapper">
        <section id="main">
            <article class="entry">
                <h2>Hubungi Kami</h2>
                <form class="contact-form">
                    <label>Nama:</label><br>
                    <input type="text" name="nama" placeholder="Masukkan nama Anda"><br><br>

                    <label>Email:</label><br>
                    <input type="email" name="email" placeholder="Masukkan email Anda"><br><br>

                    <label>Pesan:</label><br>
                    <textarea name="pesan" rows="5" placeholder="Tulis pesan Anda di sini"></textarea><br><br>

                    <button type="submit">Kirim Pesan</button>
                </form>
            </article>
        </section>

        <aside id="sidebar">
            <div class="widget-box">
                <h3 class="title">Informasi</h3>
                <p>Gunakan form ini untuk menghubungi kami melalui email.</p>
            </div>
        </aside>
    </section>

    <footer>
        <p>&copy; 2025 - Universitas Pelita Bangsa</p>
    </footer>
</div>
</body>
</html>
```
Penjelasan Halaman Kontak
```
Form diletakkan di dalam bagian utama (#main) agar sejajar dengan sidebar.
Setiap input diberi label dan placeholder agar mudah dipahami pengguna.
Tombol “Kirim Pesan” diberi warna biru dengan efek hover agar terlihat interaktif.
Tampilan halaman ini tetap konsisten dengan halaman lain karena menggunakan file CSS yang sama (style.css).
```
Tampilan halaman Kontak:
![gambar](https://github.com/MuhammadArkham/Lab4Web/blob/main/foto/Screenshot%202025-10-15%20191840.png?raw=true)
