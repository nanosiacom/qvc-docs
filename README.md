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

## Fitur

- **OpenAi GPT3** otomatis dibuatkan tulisan quote untuk video
- Tool ini menghasilkan 3 konten sekaligus.
  1. Hasilnya berupa video tentunya, di folder `results/videos`
  2. Hasilnya berupa gambar, bisa dimanfaat untuk konten ig/fb atau yg lainnya `results/images`
  3. dan yang ini berupa database di `database/database.sqlite` hasil dari OpenAi akan disimpan di database tsb. Bisa dimanfaatkan untuk caption, atau konten blog.
- Bisa tanpa OpenAi, alias manual menggunakan data quote sendiri di file `resources/quotes.txt`. Jadi sumber quotenya dari file ini.

## Untuk mendapatkan script ini langung kesini => [DISINI](https://member.nanosia.com/signup/qvc)

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

 2. Edit file `config/option.php` ganti dengan api key openai anda
 
![api key!](https://github.com/nanosiacom/qvc-docs/blob/main/api_key.png "api key")

 3. Silahkan bukan folder `resources/images` dan tambahkan image sebagai background dengan resolusi `900x1600` (recomendasi) dg aspec ratio `9:16`
 4. Dan juga silahkan buka folder `resources/audio` dan tambahkan audio untuk backsoundnya.
 5. Silahkan edit `Resources/quotes.txt` dan tambahkan atau ganti daftar quote (ini digunakan jika tidak menggunakan OpenAi)
 6. Buka laragon, klik tombol `start` dan `terminal`

![laragon!](https://github.com/nanosiacom/qvc-docs/blob/main/laragon.png "laragon")
![laragon-terminal!](https://github.com/nanosiacom/qvc-docs/blob/main/laragon-terminal.png "laragon-terminal")

 7. Di terminal jalankan perinta `php qvc go`

![php-go!](https://github.com/nanosiacom/qvc-docs/blob/main/php-go.png "php-go")
