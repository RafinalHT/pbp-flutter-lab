# counter_7

### Rafinal Haryokusumo Taloputra
### 2106634540
### PBP-F

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
