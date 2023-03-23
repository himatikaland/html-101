# HTML Fundamental by Himatika
## Menampilkan PDF di HTML
Ada 3 cara menampilkan PDF di HTML tanpa JavaScript

1. Object
2. iFrame
3. Embed

## Object
Mungkin tidak banyak yang mengetahui element ```<object>``` , dengan adanya element ini kita dapat menanamkan (embed) file PDF yang kita miliki ke dalam HTML tanpa pustaka pihak ketiga. Caranya:

1. Pastikan sudah memiliki URL file pdf yang ingin ditampilkan.
2. Tambahkan ```attribute type``` dengan value ```application/pdf```.
3. Tambahkan ```attribute data``` dengan value ```URL pdf``` yang ingin ditampilkan.
4. Set ```height``` and ```width``` sesuai keigininan.
```
<!DOCTYPE html>
<html>
  <head>
    <title>Embedding pdf - Himatika UNSIA</title>
  </head>
  <body>
    <h1>PDF Himatika UNSIA</h1>
    <object
      type="application/pdf"
      data="URL_pdf_yang_ingin_ditampilkan/sample.pdf"
      width="600"
      height="700"
    >
    </object>
  </body>
</html>
```

## iFrame
Elemen tag HTML ```<iframe>``` juga dapat digunakan untuk menampilkan halaman dalam format PDF. Cara menampilkannya yaitu dengan menyertakan nama file PDF pada atribut ```src```. 

Tampilan yang dihasilkan tiap browser untuk halaman yang sama mungkin terdapat perbedaan. Yang tidak membuat nyaman biasanya adalah nilai display (zoom) halaman PDF yang hanya 30% saja saat diakses pada browser mozilla firefox atau browser Edge.

Untuk mengatasi dapat menambahkah parameter zoom yang berfungsi sebagai pengatur display halaman PDF dengan menambahkan tanda ```#(hashtagh)``` dibelakang nama file pdf, diikuti dengan parameter-nya yaitu zoom kemudian nilai skala zoom. Misalnya display zoom 200% dilakukan dengan mengatur nilai ```zoom=200```.

Jika ingin mengatur urutan halaman yang akan tampil pertama, gunakan ```parameter page```. Misalnya halaman yang ingin ditampilkan adalah halaman ke 4 maka parameter page-nya bernilai 4.

Contoh penulisan:
```
<!DOCTYPE html>
<html>
  <head>
    <title>Embedding pdf - Himatika UNSIA</title>
  </head>
  <body>
    <h1>PDF Himatika UNSIA</h1>
    <iframe src="operating-system-concepts.pdf#page=4&zoom=200" width=100% height=800>
</iframe>
  </body>
</html>
```
## Embed
Elemen HTML tag ```<embed>``` juga dapat digunakan untuk menampilkan dokumen dalam bentuk PDF.

Cara menampilkan PDF dilakukan dengan memberi referensi dokumen format .pdf pada atribut ```SRC```. 

Contoh menampilkan dokumen PDF dimulai dari halaman 2 dengan nilai display zoom sebesar 100%.
```
<!DOCTYPE html>
<html>
  <head>
    <title>Embedding pdf - Himatika UNSIA</title>
  </head>
  <body>
    <h1>PDF Himatika UNSIA</h1>
    <embed src="css_tutorial.pdf#page=2&zoom=100" width=100% height=800></embed>
</iframe>
  </body>
</html>
```


