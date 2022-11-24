### Rafinal Haryokusumo Taloputra
### 2106634540
### PBP-F

# Tugas 7: Elemen Dasar Flutter

## Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
Stateless widget adalah widget yang tidak akan bisa berubah walaupun ada interaksi dari pengguna. Contohnya adalah Text, Icon, dan IconButton. Sedangkan, Stateful widget adalah widget yang bisa berubah dengan adanya interaksi dari pengguna. Contohnya adalah Checkbox, Radio, Slider, dll.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Text, memperbagus tulisan yang akan ditampilkan ke pengguna dengan memberikan style
2. Row and Column, menyusun isi widget secara horizontal dan vertikal
3. Container, menampung widget yang lainnya agar dapat dimodif dengan bersamaan
4. Visibility, menyembunyikan child didalamnya dengan kondisi tertentu
5. MainAxisAlignment, memposisikan children pada sumbu utama row dan column
6. Center, membuat posisi children ke tengah

## Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
Method setState() memberi tahu framework bahwa internal state dari objek telah berubah serta memicu pembaruan tampilan aplikasi. Contoh variabel yang terdampak fungsi tersebut adalah _counter.

## Jelaskan perbedaan antara const dengan final.
const dan final pada dart membuat objek tidak dapat diubah-ubah lagi. Perbedaannya adalah const membuat objek tetap pada compile-time saja dan final membuat objek tetap pada run-time

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Menambahkan method `_decrementCounter` yang akan mengurangi counter selama counter tersebut lebih dari 0
2. Membuat conditional jika counter di modulo 2 akan menghasilkan text GENAP dan jika counter di modulo 1 akan menghasilkan GANJIL serta menambahkan style color pada text
3. Menambah button decrement di bawah kiri dan menggunakan widget visibility untuk menghilangkan tombol jika counter < 1



# Tugas 8: Flutter Form

##  Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement
Navigator.push merupakan method untuk menambahkan route ke stack route yang di-manage oleh Navigator. Sedangkan, Navigator.pushReplacement Mengganti route navigator yang sedang dilihat pengguna dengan yang baru dan menambah route tersebut ke stack route navigator.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Text, memperbagus tulisan yang akan ditampilkan ke pengguna dengan memberikan style
2. Row and Column, menyusun isi widget secara horizontal dan vertikal
3. Container, menampung widget yang lainnya agar dapat dimodif dengan bersamaan
4. Visibility, menyembunyikan child didalamnya dengan kondisi tertentu
5. MainAxisAlignment, memposisikan children pada sumbu utama row dan column
6. Center, membuat posisi children ke tengah
7. Navigator, mengelola rute pada program menggunakan Stack
8. Expanded, memperluas child dari baris dan kolom untuk mengisi ruang yang ada
9. Drawer, membuat panel di sisi layar agar user bisa mengganti halaman
10. Form, wadah untuk mengelompokkan widget-widget form yang diperlukan

## Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
1. onPressed()
2. onChanged()
3. onSaved()

## Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
Navigator menggunakan struktur data stack. Stack ini digunakan untuk layar sehingga method push menampilkan top of stack dari stack layar tersebut.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Menambahkan drawer untuk menu counter, form, dan data budget
2. Menambahkan halaman form dengan input yang bisa diisi string, integer, dropdown, dan button. Input yang telah diisi akan dimasukkan kedalam list untuk disimpan agar bisa ditampilkan pada halaman budget data
3. Menambahkan halaman budget data untuk menunjukkan data yang sudah diinput pengguna dengan menggunakan ListView.Builder agar setiap objek pada list dapat ditunjukkan




# Tugas 9: Integrasi Web Service pada Flutter

## Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?
Bisa, yaitu ketika data yang ada pada JSON tidak banyak. Karena jika data JSON sudah banyak, maka jika terjadi ketidaksesuaian struktur, kita susah untuk memperbaikinya. Membuat model akan menjaga kejelasan kode dan efisiensi.

## Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya
1. Text, memperbagus tulisan yang akan ditampilkan ke pengguna dengan memberikan style
2. Row and Column, menyusun isi widget secara horizontal dan vertikal
3. Container, menampung widget yang lainnya agar dapat dimodif dengan bersamaan
4. Visibility, menyembunyikan child didalamnya dengan kondisi tertentu
5. MainAxisAlignment, memposisikan children pada sumbu utama row dan column
6. Center, membuat posisi children ke tengah
7. Navigator, mengelola rute pada program menggunakan Stack
8. Expanded, memperluas child dari baris dan kolom untuk mengisi ruang yang ada
9. Drawer, membuat panel di sisi layar agar user bisa mengganti halaman
10. Form, wadah untuk mengelompokkan widget-widget form yang diperlukan
11. Future Builder, membuat widget berdasarkan snapshot yang diambil dari Future
12. TextSpan, Menampilkan teks immutable secara merentang
13. SizedBox, Menampilkan sebuah box dengan ukuran tertentu

## Jelaskan mekanisme pengambilan data dari json hingga dapat ditampilkan pada Flutter.
Menambahkan depedensi http, kemudian melakukan GET pada data json yang selanjutnya dikonversikan ke dalam suatu model yang dibuat. Data json kemudian ditampilkan dengan menggunakan FutureBuilder.

## Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Menambahkan opsi mywatchlist pada drawer dengan ListTile
2. Membuat file dart didalam page model yang berisi code dari quicktype
3. Membuat file baru untuk memuat data-data pada tugas 3 Django dan menambahkan link data tersebut agar kita dapat mengambil dan menampilkan data menggunakan fetch
4. Menampilkan data dengan ListView.Builder dan menulis code dalam OnTap() agar film dapat ditekan dan dapat dilihat detailnya
5. Menambahkan button pada paling bawah laman detail yang akan mengembalikan pengguna ke halaman page mywatchlist
