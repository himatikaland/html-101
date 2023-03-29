Perbedaan penggunaan Class dan ID dapat dibedakan atrribut dengan menggunakan element class dan id pada sebuah tag section dan div pada html,
Class dan ID digunakan sebagai penanda kerangka pada HTML, seperti contoh penerapannya untuk mengkelompokkan nama-nama yang digunakan 
yaitu ada 4 kerangka bagian layout website seperti header, content, sidebar dan footer, kita dapat menggunakan class atau id sebagai penanda kerangkanya.

Lalu bagi seseorang yang baru mendalami, dan masih belajar tentang HTML & CSS pasti menanyakan kapan pakai ID atau Class yang tepat pada penggunaan dan penulisan tag HTML, karena attribut ID dan Class juga sama-sama di gunakan menamai tag HTML, berikut perbedaan keduanya :

ID

Atribut ID digunakan untuk penamaan elemen HTML yang memiliki karakteristik unik/berbeda. Contoh  Penerapan :

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>Demo HTML div tag id</title>
  </head>
  <body>
    <div id='header'>

    </div>

   <div id='content'>

   </div>

   <div id='sidebar'>

   </div>

   <div id='footer'>

   </div>

  </body>
</html

Kesimpulannya, bahwa kita menggunakan ID yang berbeda untuk setiap div yakni, header, content, sidebar dan footer karena semuanya memiliki struktur dan fungsi yang berbeda dalam suatu dokumen HTML.

Class

Class digunakan untuk penamaan elemen yang memiliki karakteristik/struktur sama dan dapat digunakan berulang kali dalam markup (Kode HTML). Sebagai contoh, perhatikan kode HTML berikut :

<ul id='menu'>
     <li class='merah'>Beranda</li>
     <li>Tutorial</li>
     <li class='merah'>Berita</li>
     <li>Galeri</li>
</ul>

Pada Kode HTML di atas, saya menggunakan class Merah pada beberapa list item, karena nantinya list item yang memiliki class merah akan diberi warna background merah.

Kesimpulannya adalah, ketika anda memiliki beberapa elemen dengan karakter/format yang sama, gunakan Class sebagai penamaannya dan Gunakan ID untuk elemen yang berbeda dan membutuhkan tanda pengenal lebih spesifik.
