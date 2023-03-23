# HTML Fundamental by Himatika
## Apa itu Video Player HTML?
Pada HTML4 dan versi HTML lawas lainnya, file video hanya bisa ditambahkan pada website menggunakan plugin multimedia seperti Adobe Flash.

HTML5 terdapat tags khusus bernama HTML5 video player ```<video>...</video>``` yang mendukung tiga format file video untuk web, yakni MP4, Ogg dan WebM.
Tag video player memungkinkan penyematan video secara langsung ke berbagai halaman situs dan dapat mencantumkan sumber video eksternal berupa file atau URL.

## Menggunakan tag ```<video>```
Kita bisa langsung menggunakan tag ```<video>...</video>``` dengan syarat sudah memiliki sumber video. Menetapkan sumber file video bisa dilakukan memakai atribut ```HTML src```, namun lebih disarankan untuk memilih tag ```<source>``` saja.  Tags ```<source>``` dianggap lebih baik karena memungkinkan untuk multiple source, sedangkan attribut ```src``` tidak.

Contoh Codingannya:
```<video>
<!DOCTYPE html>
<html>
<head>
    <title>Cara Bikin Pemutar Video di HTML - Himatika UNSIA</title>
</head>
<body>
    <h1>Contoh Video Yang di Putar - Himatika UNSIA</h1>
    <br>
    <video width="400px" height="350px" controls>
        <source src="https://youtu.be/GER09e14lcA" type="video/mp4">
    </video>
    
</body>
</html>
```
* File video bisa disimpan pada folder yang sama dengan file HTML maupun terpisah. Apabila terpisah, tambahkan ```../nama_folder/nama_video```.
* File video dalam folder yang sama dengan file HTML, namun disimpan didalam sebuah folder, tambhakan ```/nama_folder/nama_video```.
* File video dalam folder yang sama dengan file HTML panggil langsung nama dari file video yang ingin diputar.

## Control Video Player
Panel kontrol video player memuat berbagai tombol untuk mengatur jalannya video. Misalnya memulai tayangan (play), menjeda (pause), menghentikan (stop), melompati bagian tertentu (skip), beralih antar jendela (switch) hingga menampilkan video layar penuh (full screen).

Cukup sertakan atribut ```controls``` untuk melakukannya. Contohnya seperti berikut:
```
<video controls width="700" height="500">
  <source src="https://youtu.be/GER09e14lcA" type="video/mp4">
  Tag video tidak didukung oleh browser
</video>
```
Jika video memiliki suara, maka secara otomatis panel kontrol HTML5 akan menyediakan opsi modifikasi volume suara (up or down volume), atau bahkan membisukannya (mute).

## Mengatur Ukuran Video Player
Gunakan atribute HTML ```height``` dan ```width``` untuk mengatur ukuran dari video player. Secara otomatis video akan mempertahankan ukurannya dalam rasio yang sama.

Pengaturan ukuran player juga bermanfaat untuk menghindari flickering (layar berkedip) selama proses loading.

Pada contoh koding berikut, nilai atribut height (tinggi) diatur sebesar 700, dan width (lebar)-nya adalah 500:
```
<video controls width="700" height="500">
  <source src="https://youtu.be/GER09e14lcA" type="video/mp4" width="700" height="500">
  Tag video tidak didukung oleh browser
</video>
```

## Tips n trik
* Tambahkan ```atribut type``` jika menggunakan elemen ```<source>``` untuk menghindari pembuangan waktu/upaya loading karena browser secara otomatis mengabaikan format-format file yang tidak didukung.
*  ```atribut poster``` untuk menambahkan gambar thumbnail sebelum video diputar.
* Kostumasi tampilan video player lebih lanjut memakai CSS, seperti menambahkan border dan mengatur opacity.
* Browser komputer yag mendukung: ```Firefox, Chrome, Opera, Internet Explorer dan Safari```.
* Browser smartphone yang mendukung: ```Firefox, Chrome, Opera, dan Safari```.
