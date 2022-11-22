# counter_7

### Link to TUGAS 8 [Here](#tugas-8)
### Link to TUGAS 9 [Here](#tugas-9)

---

# TUGAS 7

1. *Stateless widget* adalah widget yang `state` nya tidak dapat diubah setelah widgetnya dibuild. Sedangkan *stateful widgets* adalah widget yang dapat diubah `state`nya setelah widghetnya dibuild. Perbedaan antara keduanya adalah *stateless widget* merupakan widget yang *static* sedangkan *stateful widget* adalah widget *dynamic*. *Stateless widget* tidak bergantung pada perubahan data atau *behaviour*. Sedangkan *statefull widget* bisa diupdate saat *runtime* berdasarkan perubahan data atau *user-action*.
<br>

2. Widget yang digunakan di proyek ini adalah: 
   1. `MaterialApp` yang berfungsi mengkonfigurasi widget Navigator atau Theme.
   2. `Scaffold` yang menyediakan banyak widget lainnya. Scaffold akan menempati seluruh screen dari device.
   3. `AppBar` yaitu bar yang ada di paling atas dan berisi judul proyek untuk kali ini.
   4. `Text` yaitu widget yang berisi text dengan satu styling.
   5. `Center` yaitu widget yang memusatkan(centers) child-childnya.
   6. `Column` yaitu widget yang menata child-childnya dalam susunan vertikal
   7. `Padding` yang memberikan padding pada child-childnya.
   8. `Row` yaitu widget yang menata child-childnya dalam susunan horizontal
   9. `FloatingActionButton` yaitu button yang menghover diatas konten dan memiliki fungsi onPressed
<br>

3. `setState()` memungkinkan sebuah widget untuk di rebuild sehingga variabel value yang ada dapat diganti. Variabel yang terdampak adalah variabel tidak final yang ada di class yang sama dengan pemanggilan setState tersebut.
<br>

4. `const` memiliki *behaviour* yang sama seperti `final` akan tetapi `const` membuat variabel tersebut constant dari compile-time saja.
<br>

5. Pertama buat flutter app bernama `counter_7`, lalu ganti title di `MaterialApp` dan juga title yang ada di `AppBar`. Lalu buat fungsi untuk decrement counter pada class `_MyHomePageState` dimana fungsinya memanggil `setState()` lalu didalam `setState()` cek apakah _counter bernilai 0, jika tidak maka _counter--. Setelah itu ubah text diatas text counter dengan mengecek apakah _counter ganjil atau genap dan assign string dan style textnya sesuai yang diminta pada soal. Lalu buat dua `FloatingActionButton` dengan `FloatingActionButtonLocation.centerDocked` dan kedua button tersebut berada dalam `Row` yang di align `spaceBetween`. Satu button memiliki fungsi decrement dan satunya memiliki fungsi increment.
    
---

# TUGAS 8

1. `Navigator.push` mendorong route yang diberikan keatas stack sehingga muncul tampilan dari route tersebut tanpa menghilangkan route yang sebelumnya. Sedangkan `Navigator.pushReplacement` mendorong route yang diberikan keatas stack sehingga tampilan dari route tersebut muncul dan menghilangkan route yang sebelumnya sehingga tampilan awalnya tergantikan dengan yang baru setelah animasinya selesai.
   <br>

2. Widget yang digunakan di proyek ini adalah: 
   1. `MaterialApp` yang berfungsi mengkonfigurasi widget Navigator atau Theme.
   2. `Scaffold` yang menyediakan banyak widget lainnya. Scaffold akan menempati seluruh screen dari device.
   3. `AppBar` yaitu bar yang ada di paling atas dan berisi judul proyek untuk kali ini.
   4. `Text` yaitu widget yang berisi text dengan satu styling.
   5. `Center` yaitu widget yang memusatkan(centers) child-childnya.
   6. `Column` yaitu widget yang menata child-childnya dalam susunan vertikal
   7. `Padding` yang memberikan padding pada child-childnya.
   8. `Row` yaitu widget yang menata child-childnya dalam susunan horizontal
   9. `Drawer` yaitu widget yang biasanya digunakan sebagai side menu
   10. `ListView` yaitu widget yang akan menunjukan children nya satu-persatu searah dengan arah scroll
   11. `ListTile` yaitu widget yang dapat berisi 1 sampai 3 baris text yang tiap barisnya dapat disandingkan dengan icon ataupun widget lain.
   12. `Card` yaitu widget yang digunakan sebagai container untuk widget lain yang memiliki rounded-edge dan dapat berupa elevated, outlined, ataupun filled card.
   13. `Navigator` yaitu widget yang digunakan untuk mengarahkan ke route lain (contoh: menunjukan page lain)
   14. `SizedBox` yaitu widget berupa box yang memiliki ukuran sesuai dengan yang diberikan yang digunakan sebagai container widget lain
   15. `DropdownButtonFormField` yaitu widget form berupa dropdown
   16. `DropdownMenuItem` yaitu widget untuk menunjukan item-item pada dropdown
   17. `TextFormField` yaitu widget untuk menerima input text
   18. `InputDecoration` yaitu widget untuk menambahkan decoration pada input
   19. `SingleChildScrollView` yaitu widget yang memungkinkan untuk melakukan scroll pada isi widget tersebut
<br>

3. Event yang ada di Flutter: 
   1. `onPressed`
   2. `onChanged`
   3. `onTap`
   4. `onSaved`
<br>

4. `Navigator` akan menangani route-route yang ada dan akan menambahkan route dari page yang akan ditampilkan keatas `stack of route` sehingga page berada di paling atas.
   <br>

5. Buat drawer yang akan digunakan sebagai menu untuk berpindah halaman dan tambahkan route ke tiap halaman. Buat class `MyBudget` dengan fields judul, nominal, dan jenis serta static field berupa list yang berisi objek `MyBudget` untuk menyimpan data tiap budget yang diinput. Dalam `form.dart` buat Body yang berisi `Form()` dan tambahkan `formKey` untuk validasi input serta buat input-inputnya yang berupa `TextFormField` dan `DropdownButtonFormField`. Tambahkan decoration untuk tiap input agar lebih deskriptif. Setelah itu berikan fungsi `onChanged` dan `onSaved` untuk menyimpan data yang diinput. Tambahkan button untuk menyimpan data dengan fungsi `onPressed` yang akan melakukan validasi input, jika input valid maka akan data yang diinput akan disatukan menjadi objek `MyBudget` dan ditambahkan ke `listBudget` serta akan memunculkan `dialog` berisi pemberitahuan bahwa input nya berhasil disimpan. Untuk `data.dart`, dengan menggunakan `ListView.builder` akan dibuat card untuk tiap objek yang ada di `listbudget`.

---

# TUGAS 9

1. Kita tidak dapat mengambil data JSON tanpa membuat model nya terlebih dahulu karena kita tidak bisa menyatukan field-field yang ada di tiap data yang diambil kedalam satu *class* sehingga fields-fields nya tidak dapat diakses
   <br>

2. Widget yang digunakan di proyek ini adalah: 
   1. `MaterialApp` yang berfungsi mengkonfigurasi widget Navigator atau Theme.
   2. `Scaffold` yang menyediakan banyak widget lainnya. Scaffold akan menempati seluruh screen dari device.
   3. `AppBar` yaitu bar yang ada di paling atas dan berisi judul proyek untuk kali ini.
   4. `Text` yaitu widget yang berisi text dengan satu styling.
   5. `Center` yaitu widget yang memusatkan(centers) child-childnya.
   6. `Column` yaitu widget yang menata child-childnya dalam susunan vertikal
   7. `Padding` yang memberikan padding pada child-childnya.
   8. `Row` yaitu widget yang menata child-childnya dalam susunan horizontal
   9. `Drawer` yaitu widget yang biasanya digunakan sebagai side menu
   10. `ListView` yaitu widget yang akan menunjukan children nya satu-persatu searah dengan arah scroll
   11. `ListTile` yaitu widget yang dapat berisi 1 sampai 3 baris text yang tiap barisnya dapat disandingkan dengan icon ataupun widget lain.
   12. `Card` yaitu widget yang digunakan sebagai container untuk widget lain yang memiliki rounded-edge dan dapat berupa elevated, outlined, ataupun filled card.
   13. `Navigator` yaitu widget yang digunakan untuk mengarahkan ke route lain (contoh: menunjukan page lain)
   14. `SizedBox` yaitu widget berupa box yang memiliki ukuran sesuai dengan yang diberikan yang digunakan sebagai container widget lain
   15. `CircularProgressIndicator`, widget yang menunjukan sebuah progres dalam sebuah lingkaran yang berputar, dapat digunakan untuk loading screen
   16. `FutureBuilder` adalah widget untuk membantu proses asinkronus yang akan mengupdate tampilan berdasarkan hasil proses asinkronus tersebut
   17. `InkWell` widget yang akan memenuhi sebuah material widget agar dapat merespon *touch events* seperti `onTap`.
   18. `Expanded` yaitu widget yang akan memperluas `child` dari `Row`,`Column`, atau `Flex` agar memenuhi ruang yang tersisa dalam *main axis* nya
   19. `Checkbox` yaitu material widget berupa checkbox
<br>

3. Mekanisme pengambilan data JSON di Flutter: 
   1. Buat model dari data yang akan diambil yang berisi fields-fields yang ada dalam setiap data tersebut.
   2. Import `dart:convert` pada file berisi model tersebut agar dapat mengkonversi data dari dan ke JSON.
   3. Buat fungsi untuk mengambil data dari web service yang berisi data JSON tersebut dengan men-decode JSON tersebutr menjadi model yang telah dibuat dan disatukan kedalam list.
   4. Import `model` yang telah dibuat, `http.dart`, dan `dart:convert` di file yang berisi fungsi tersebut.
   5. Untuk mengambil dan menampilkan data, gunakan `FutureBuilder` dengan future yang didapat dengan memanggil fungsi yang dibuat tadi.
   6. data yang didapat sudah bisa ditampilkan.
<br>

4. Step-by-step mengimplementasikan Tugas 9:
   1. Membuat `MyWatchlistPage` dan menambahkan nya ke drawer navigasi
   2. Membuat model `Mywatchlist`
   3. Menampilkan seluruh judul yang ada di database watchlist dengan melakukan pengambilan data dari JSON yang dibuat di Tugas 3 dengan menggunakan fungsi yang telah dibuat dengan nama `fetchWatchlist` dan jadikan hasil dari fungsi tersebut sebagai `future` dari `FutureBuilder`
   4. Tambahkan fungsi onTap pada `InkWell` yang meliputi tiap judul yang akan menavigasikan ke halaman detail
   5. Buat `DetailPage` dengan mem-pass data dari `MyWatchlistPage` dan tampilkan detail dari data mywatchlist tersebut
   6. tambahkan button yang akan melakukan `pop` di `DetailPage` sehingga akan kembali ke `MyWatchlistPage`.
   7. tambahkan `Checkbox` pada setiap judul watchlist di `MyWatchlistPage` yang akan merubah value `watched` dari data `Mywatchlist` dan akan merubah warna text dan outline yang ditampilkan.
   <br>