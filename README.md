# counter_7

1. *Stateless widget* adalah widget yang `state` nya tidak dapat diubah setelah widgetnya dibuild. Sedangkan *stateful widgets* adalah widget yang dapat diubah `state`nya setelah widghetnya dibuild. Perbedaan antara keduanya adalah *stateless widget* merupakan widget yang *static* sedangkan *stateful widget* adalah widget *dynamic*. *Stateless widget* tidak bergantung pada perubahan data atau *behaviour*. Sedangkan *statefull widget* bisa diupdate saat *runtime* berdasarkan perubahan data atau *user-action*.<br>
2. Widget yang digunakan di proyek ini adalah
    - `MaterialApp` yang berfungsi mengkonfigurasi widget Navigator atau Theme.
    - `Scaffold` yang menyediakan banyak widget lainnya. Scaffold akan menempati seluruh screen dari device.
    - `AppBar` yaitu bar yang ada di paling atas dan berisi judul proyek untuk kali ini.
    - `Text` yaitu widget yang berisi text dengan satu styling.
    - `Center` yaitu widget yang memusatkan(centers) child-childnya.
    - `Column` yaitu widget yang menata child-childnya dalam susunan vertikal
    - `Padding` yang memberikan padding pada child-childnya.
    - `Row` yaitu widget yang menata child-childnya dalam susunan horizontal
    - `FloatingActionButton` yaitu button yang menghover diatas konten dan memiliki fungsi onPressed
<br>
3. `setState()` memungkinkan sebuah widget untuk di rebuild sehingga variabel value yang ada dapat diganti. Variabel yang terdampak adalah variabel tidak final yang ada di class yang sama dengan pemanggilan setState tersebut.<br>
4. `const` memiliki *behaviour* yang sama seperti `final` akan tetapi `const` membuat variabel tersebut constant dari compile-time saja.<br>
5. Pertama buat flutter app bernama `counter_7`, lalu ganti title di `MaterialApp` dan juga title yang ada di `AppBar`. Lalu buat fungsi untuk decrement counter pada class `_MyHomePageState` dimana fungsinya memanggil `setState()` lalu didalam `setState()` cek apakah _counter bernilai 0, jika tidak maka _counter--. Setelah itu ubah text diatas text counter dengan mengecek apakah _counter ganjil atau genap dan assign string dan style textnya sesuai yang diminta pada soal. Lalu buat dua `FloatingActionButton` dengan `FloatingActionButtonLocation.centerDocked` dan kedua button tersebut berada dalam `Row` yang di align `spaceBetween`. Satu button memiliki fungsi decrement dan satunya memiliki fungsi increment.



