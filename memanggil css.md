Artikel ini menjelaskan tentang bagaimana memanggil CSS ke dalam HTML. 
apa sih CSS itu? CSS (Cascading Style Sheets) adalah suatu bahasa stylesheet yang digunakan untuk mengatur tampilan suatu dokumen yang ditulis dalam bahasa markup. 
Penggunaan yang paling umum dari CSS adalah untuk memformat halaman web yang ditulis dengan HTML dan XHTML.

Terdapat 3 cara untuk memanggil CSS :

1. Membuat File CSS terpisah dengan HTML

2. Menyisipkan perintah CSS diantara tag

3. Menyisipkan perintah CSS di dalam perintah-perintah HTML.


Caranya yaitu : 

1. Membuat File CSS terpisah dengan HTML.

Untuk membuat file CSS terpisah dengan HTML, Anda bisa membuat file dengan format .CSS dan setelah itu memanggil file Anda dalam HTML. 
Sebagai contoh, saya akan membuat file yang akan saya beri nama style.css,seperti ini:

Contoh 

Buat file css dengan nama style.css

body {
    margin:0;
    padding:0;
}

h1 {
    font-size:1.6em; 
    font-weight:normal;
}


Kemudian untuk memanggil style CSS diatas gunakan perintah

<link href="style.css" rel="stylesheet" type="text/css">



2. Menyisipkan perintah CSS diantara tag

Cara lain adalah dengan menyisipkan baris kode CSS di antara tag

<html>
    <head>
        <style>
        body {
            margin:0;
            padding:0;
        }

        h1 {
            font-size:1.6em; 
            font-weight:normal;
        }
        </style>
    </head>
</html>



3. Menyisipkan perintah CSS ke dalam perintah-perintah HTML

Maksudnya adalah menyisipkan perintah perintah CSS di dalam perintah HTML, Contoh :

<h1 style="font-size:1.6em; font-weight:normal;">Heading 1</h1>
