# HTML Fundamental By HIMATIKA

## Menampilkan Sebuah Image
di HTML, untuk menampilkan sebuah image kita bisa menggunakan tag `<img>` <br>
Tag ini terdiri dari beberapa atribut yang dapat digunakan untuk menentukan sumber gambar, deskripsi alternatif, ukuran gambar, dan lain-lain.

## Atribut
Berikut ini adalah atribut yang dapat digunakan pada tag `<img>`:

- src : atribut wajib yang menunjukkan URL atau path dari gambar yang ingin ditampilkan.<br><br>
- alt : atribut opsional yang memberikan deskripsi alternatif tentang gambar, yang berguna jika gambar tidak dapat ditampilkan atau jika pengguna menggunakan pembaca layar.<br><br>
- width : atribut opsional yang menunjukkan lebar gambar dalam piksel atau persentase. Jika tidak ditentukan, maka ukuran gambar akan menyesuaikan dengan ukuran aslinya.<br><br>
- height : atribut opsional yang menunjukkan tinggi gambar dalam piksel atau persentase. Jika tidak ditentukan, maka ukuran gambar akan menyesuaikan dengan ukuran aslinya.<br><br>
- loading : atribut opsional yang menunjukkan bagaimana gambar harus dimuat. Nilai yang dapat digunakan adalah "lazy" (untuk memuat gambar hanya ketika gambar muncul di tampilan) atau "eager" (untuk memuat gambar segera saat halaman dimuat).<br><br>
- decoding : atribut opsional yang menunjukkan bagaimana gambar harus di-decode. Nilai yang dapat digunakan adalah "sync" (untuk meng-decode gambar segera saat gambar dimuat) atau "async" (untuk meng-decode gambar secara asinkron setelah halaman dimuat).<br><br>
- crossorigin : atribut opsional yang menunjukkan apakah gambar harus dimuat dengan atribut CORS. Nilai yang dapat digunakan adalah "anonymous" (untuk memuat gambar tanpa menyertakan kredensial pengguna) atau "use-credentials" (untuk memuat gambar dengan menyertakan kredensial pengguna).<br><br>
- usemap : atribut opsional yang menunjukkan nama peta gambar (map) yang berisi area-area yang dapat diklik pada gambar tersebut.<br><br>

## Contoh Penggunaan
```
<!DOCTYPE html>
<html>
  <head>
    <title>Contoh Gambar</title>
  </head>
  <body>
        <img src="https://i.pinimg.com/564x/88/8d/b0/888db0062b1b2d0d8e5d208dc7255232.jpg" alt="Kucing" />
  </body>
</html>
```
### Output
<img src="https://i.pinimg.com/564x/88/8d/b0/888db0062b1b2d0d8e5d208dc7255232.jpg" alt="Kucing" />
<br>
<br>
Pada contoh di atas, gambar kucing ditampilkan dengan menggunakan tag `<img>` dengan atribut src yang menunjukkan URL dari gambar kucing di atas. Atribut alt juga digunakan untuk memberikan deskripsi alternatif tentang gambar.
