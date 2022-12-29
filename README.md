# Tugas Akhir VIX Frontend Developer di Core Initiative batch Desember 2022

## Deskripsi
Pada task terakhir VIX Front End Developer Core Initiative ini, kalian diberikan tugas untuk membentuk sebuah interface dari sebuah website Ecommerce. Kalian ditugaskan untuk membuat dua halaman yaitu men's clothing dan woman's clothing. Pada task ini, kalian akan bekerja dengan tim UI/UX dan juga tim Backend, sehingga website yang akan kalian bangun telah memiliki komponen design juga code API nya.

## Ketentuan Tugas
1. Menampilkan data yang didapat dari API https://fakestoreapi.com dengan index merupakan angka 1-20 yang di tiap index-nya memiliki kategori yang berbeda, misalnya https://fakestoreapi.com/products/1 yang memiliki kategori men’s clothing
2. Produk yang ditampilkan hanya 1, namun akan berubah setiap kali user menekan tombol Next Product
3. Sediakan loading element/loader yang akan ditampilkan ketika menunggu balasan dari API sehingga desain tetap UX friendly. Loader bisa berupa [spinner](https://www.w3schools.com/howto/howto_css_loader.asp) atau [skeleton](https://dev.to/devggaurav/build-a-simple-card-skeleton-loader-component-using-html-andcss-3a20)
4. Membentuk tiga halaman website sesuai dengan desain yang telah di sediakan di Figma [berikut ini](https://www.figma.com/file/x1bkO3alpmGQFtysh9Lmn7/Task-5-Ecommerce?node-id=0%3A1)

## API Call:
1. Kalian akan mengakses sebuah API sebuah ecommerce, 
2. Silakan membuka https://fakestoreapi.com/docs untuk mendapatkan informasi mengenai API E-Commerce ini
3. Pada projek VueJS yang telah dibuat, silakan fetch API dengan endpoint https://fakestoreapi.com/products/index yang mana index adalah angka 1-20
4. Panggil API saat user menekan tombol Next Product, silakan gunakan increment untuk menambah index di setiap user menekan tombol tersebut. Index inilah yang nanti digunakan untuk fetch API di step nomor 2
5. Setelah mendapat balasan dari API, gunakan kondisi untuk mengecek jika category = men’s clothing atau category = women’s clothing, maka simpan balasan tersebut pada variable yang telah dibuat di data(), jika category selain 2 di atas, maka jangan simpan balasannya
6. Untuk menghindari error saat fetch API, ketika index sudah mencapai 20, maka atur index supaya kembali ke 1 karena API hanya menyediakan 20 jenis produk

## Komponen Desain:
1. Terdapat 3 macam desain: men section, women section, dan unavailable product
2. Aplikasikan desain menggunakan Vanilla CSS (CSS tanpa framework)
3. Untuk memudahkan silakan buat variable pada CSS untuk menampung color palette yang sudah disediakan di section Color Palette di Figma
4. Pada projek Vue yang telah dibuat, gunakan class binding untuk mengecek jika category = men’s clothing maka gunakan class CSS yang berkaitan dengan desain Page-Men section, jika category = women’s clothing, menggunakan class CSS yang berkaitan dengan desain Page-Women section, jika category selain 2 di atas, menggunakan class CSS yang berkaitan dengan desain Page-Unavailable product


## Hasil Projek yang dibuat
Dapat membuat Interface sesuai desain di figma, serta dapat menampilkan data produk yang ada pada API. dibuat dengan : Framework JavaScript Vue js & Vanila CSS.

Beberapa fitur yg belum selesai :
- Menampilkan banyak card produk, bukan satu card produk yg bisa di klik next. Jadi tombol next juga belum berfungsi
- Kesesuaian warna dengan kategori
- simbol atau icon rating
