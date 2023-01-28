# Quote Video Creator

Quote Video Creator adalah sebuat tool untuk membuat video yang bertipe Quote dan sudah di dukung dengan tehnologi **OpenAi Gpt3** yang bisa membuatkan sebuah Quote untuk dijadikan sebuah video pendek, video bisa di unggah ke social media seperti Tiktok, Ig/Fb Reel, Youtube Short, dsb.

Saya terinspirasi dengan beberapa video di youtube, yang membagikan sebuah cara untuk mendapatkan penghasilan dengan youtube short, dan sekaligus mendapatkan pahala.

![inspirasi!](https://github.com/nanosiacom/qvc-docs/blob/main/inspirasi.png "inspirasi")

Dari ss diatas, terlihat penghasilan mereka antara `14juta`, `20juta`, `sampai 90juta`. 

Akhirnya saya membuat sebuah tool untuk mempermudah dalam pembuatan konten untuk video shortnya.

Contoh hasil videonya seperti ini:
- https://www.youtube.com/shorts/eY-d8rTgz9o
- https://www.youtube.com/shorts/o4a9ezangHg
- https://www.youtube.com/shorts/TQeE86M4DV8

## Alat dan Bahan
1. Php >=8.1 (Windows Laragon)
2. FFmpeg

## Tahap Instalasi

### Install PHP 8.1 Laragon
  1. Download laragon [disini](https://laragon.org/download/index.html), pilih laragon full, kemudian install seperti instalasi software yg lain.

![laragon-download!](https://github.com/nanosiacom/qvc-docs/blob/main/laragon-download.png "laragon-download")

  2. Download php 8.1 [disini](https://windows.php.net/download) , pilih yg Thread Safe

![php-download!](https://github.com/nanosiacom/qvc-docs/blob/main/php-download.png "php-download")

  3. Buka folder `laragon-bin-php`, yang biasanya berlokasi di `C:\laragon\bin\php`. Paste php 8.1 yang sudah didownload sebelumnya, kemudian extract
  
![php81!](https://github.com/nanosiacom/qvc-docs/blob/main/php81.png "php81")

  4. Buka laragon, klik kanan, kemudian pilih PHP-version-centang php 8.1.14
  5. Masih di laragon, lakukan klik kanan, kemudian pilih **PHP-Extensions-pastikan** centang bagian **pdo_sqlite**

### Install FFmpeg
  1. Download FFmpeg [disini](https://www.gyan.dev/ffmpeg/builds/)

![ffmpeg-download!](https://github.com/nanosiacom/qvc-docs/blob/main/ffmpeg-download.png "ffmpeg-download")

  2. Selanjutnya memasukkan lokasi `C:\ffmpeg\bin` ke Path Windows. caranya ikuti pada video berikut ini https://www.youtube.com/watch?v=cnRAO9b0LHE
  3. Jangan lupa restart windows.

## Penggunaan

 1. Extract file `quote-video-creator.zip` 

![quote-video-creator!](https://github.com/nanosiacom/qvc-docs/blob/main/qvc.png "quote-video-creator")

 3. Buka laragon, klik tombol `start` dan `terminal`

![laragon!](https://github.com/nanosiacom/qvc-docs/blob/main/laragon.png "laragon")
![laragon-terminal!](https://github.com/nanosiacom/qvc-docs/blob/main/laragon-terminal.png "laragon-terminal")

 3. Di terminal jalankan perinta `php qvc go`

![php-go!](https://github.com/nanosiacom/qvc-docs/blob/main/php-go.png "php-go")
