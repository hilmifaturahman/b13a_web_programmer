■ DOM merupakan singkatan dari Document Object Model. Artinya, dokumen(HTML) yang dimodelkan dalam sebuah objek.
■ Objek dari dokumen ini menyediakan sekumpulan fungsi dan atribut/data yang bisa kita manfaatkan dalam membuat program javascript. Inilah yang di sebut API(Application Programming Interface)
■ Objek DOM di javascript bernama document. Objek ini berisi segala hal yang kita butuhkan untuk memanipulasi HTML.
■ Jika kita coba ketik document pada console javascript, maka yang akan tampil adalah kode HTML.
■ didalam objek dockument, terdapat fungsi-fungsi dan atribut yang bisa kita gunakan untuk memanipulasi dokumen HTML.
■ Sebagai contoh fungsi document.write().
  ■ Fungsi ini digunakan untuk menulis sesuatu ke dalam HTML.
  ■ contoh:
  document.write("Hello World YAL");
  document.write("<h2>Saya Sedang Belajar DOM</h2>");
  hasilnya akan langsung berdampak pada dokumen HTML
__________________________________________________________________________________
■ Mengakses elemen tertentu dengan DOM
  ■ contoh:
  // mengakses objek head
  document.head;

  // mengakses objek body
  document.body;

  // melihat jumlah huruf di judul pada objek title
  document.title.length;
__________________________________________________________________________________
■ Apabila kita ingin mengakses elemen yang spesifik, terdapat beberapa fungsi yang bisa di gunakan:
  ■ getElementById() fungsi untuk memilih elemen berdasarkan atribut id.
  ■ getElementByName() fungsi untuk memilih elemen berdasarkan atribut name.
  ■ getElementByClassName() fungsi untuk memilih elemen berdasarkan atribut class.
  ■ getElementByTagName() fungsi untuk memilih elemen berdasarkan nama tag.
  ■ getElementByTagNameNS() fungsi untuk memilih elemen berdasarkan nama tag.
  ■ querySelector() fungsi untuk memilih elemen berdasarkan query.
  ■ querySelectorAll() fungsi untuk memilih elemen berdasarkan query.
__________________________________________________________________________________
■ Membuat Elemen dengan DOM API
DOM juga menyediakan fungsi untuk membuat elemen HTML.
■ Salah satunya adalah fungsi createElement().
  ■ Contoh:
  document.createElement('p');

  maka akan tercipta emelent <p> baru. Namun tidak ditampilkan ke dalam halaman web.
  ■ Mengapa tidak ditampilkan?
  karena kita belum menambahkannya ke dalam body dokumen.
  ■ Cara menambakannya ke body document, kita bisa gunakan fungsi append()
__________________________________________________________________________________
  ■ contoh:
  <!DOCTYPE html>
  <html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
  </head>

  <body>
    <script>
      // membuat element h1
      var judul = document.createElement("h1");
      
      // mengisi konten element
      judul.textContext = "Belajar Javascript";
      
      // menambahkan element ke dalam tag body
      document.body.append(judul);
    </script>
  </body>
  </html>
__________________________________________________________________________________
■ Menghapus elemen dengan DOM API
■ untuk menghapus element kita bisa gunakan fungsi remove()
  ■ contoh:
  <!DOCTYPE html>
  <html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>DOM Javascript</title>
  </head>

  <body>

    <h2 id="judul2">Delete Saya!</h2>
    
      <script>
      // memilih element berdasarkan Id
      var h2 = document.getElementById("judul2");
      
      // menghapus elemen yang sudah dipilih
      h2.remove();
      
      console.log("Elemen sudah dihapus")
      console.log(h2);
      </script>
    </body>
    </html>
	
	  Element berhasil dihapus dari halaman web, namun elemen masih berada di dalam memori.
__________________________________________________________________________________	
■ Contoh program menggunakan DOM:
	<!DOCTYPE html>
  <html lang="en">

  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>DOM Javascript</title>
  </head>

  <body>
    <h1>Aplikasi Ubah Warna</h1>
    <label>Warna latar: </label>
    <input type="color" id="bg-color" />
    <br>
    <label>Warna teks: </label>
    <input type="color" id="text-color" />
    
    <script>
      var bgColor = document.getElementById("bg-color");
      vat txtColor = document.getElementById("text-color");
      
      bgColor.addEventListener("change", (event) => {
      document.body.style.backgroundColor = bgColor.value;
    });
    
    txtColor.addEventListener("change", (event) => {
      document.body.style.color = textColor.value;
    });
    </script>
  </body>
  </html>

  ■ kita menggunakan event "change" pada element bgColor dan txtColor artinya nanti setiap nilai dari elemen ini berubah, kode didalamnya akan dieksekusi.
__________________________________________________________________________________
■ Regular Expression atau sering disingkat RegExp atau RE adalah suatu mekanisme pencocokan pola(pattern matching) yang dibuat dengan menggunakan karakter-karakter khusus. Fungsinya sangat beragam, mulai dari memeriksa apakah sebuah inputan sudah sesuai atau belum (test), untuk  membuat fitur pencarian(search) atau penggantian string(replace).
■ Contoh method yang menggunakan RegExp Diantaranya method search(), match() dan replace(). Selain itu juga terdapat beberapa method yang khusus "melekat" ke RegExp Object javascript.
■ Penggunaan paling banyak dari RegExp adalah untuk proses validasi form. Sebagai contoh, bagaimana caranya kita memastikan seseorang sudah menginput alamat email dengan benar? Apakah yang diinput di kolom total pemesanan sudah berupa angka? atau malah huruf? Bagaimana cara memastikan inputan password yang syaratnya harus dibuat dari 6 karakter dan mengandung minimal 1 angka dan 1 huruf besar? Ini semua ditangani oleh RegExp.
__________________________________________________________________________________
■ Cara Membuat RegExp Object
Di dalam javascript, regular expression ditempatkan ke dalam object sendiri, yakni RegExp object. ada 2 cara penulisan yaitu menggunakan object constructor atau cara langsung (literal).

■ Berikut contoh pembuatan RegExp di dalam javascript:
  var foo = /ab+c/;

  console.log(foo); // /ab+c/
  console.log(typeof foo); // object

  var bar = new RegExp("ab+c");

  console.log(bar); // /ab+c/
  console.log(typeof bar); // object
__________________________________________________________________________________
■ Menggunakan penulisan literal, kita tinggal membuat pola karakter diantara tanda forward slash: / dan /. Ini merupakan cara membuat regexp yang paling disarankan.
■ Menggunakan object constructor, perintahnya adalah new RegExp(). Dimana pola regular expression diinput sebagai argumen dari RegExp(). Cara ini tidak sering dipakai karena kurang efisien jika dibandingkan penulisan literal. Namun apabila pola regular expression diinput secara realtime (misalnya kode regexp diinput langsung dari form). Penulisan object contructor bisa dipakai.
__________________________________________________________________________________
■ RegExp Object Method
RegExp object memiliki beberapa method dan property. Sebagian besar dari method ini merupakan fitur lanjutan yang jarang dipakai. Kita hanya akan membahas 2 diantaranya: method test() dan exec().
  ■ Method RegExp.prototype.test()
  Method test() digunakan untuk memeriksa apakah sebuah string lolos dari pola regular expression yang diinput. Jika lolos, hasilnya true. Jika tidak, hasilnya false.
  ■ Method ini mirip seperti include() dari String Object. Bedanya pada method test() pengecekan string menggunakan pola regular expression. Berikut contoh penggunaannya:

    var foo = "Belajar Javascript";
    var pola = /JavaScript/;

    console.log(pola.test(foo)); // true
    console.log(/Belajar/.test(foo)); // true
    consloe.log(/belajar/.test(foo)); // false

    ■ Disini kita membuat 2 buah variabel: foo dan pola. Variabel foo berisi string sedangkan pola berisi pola regular expression /JavaScript/.
    ■ Perintah pola.test(foo) artinya kita ingin memeriksa apakan pola /JavaScript/ terdapat di dalam string foo atau tidak. Pola `/JavaScript/ `maksudanya sama dengan sebuah kata "JavaScript". Kata ini tentunya ada di dalam variabel foo dan hasil method test() adalah true.
    ■ Begitu juga dengan perintah /Belajar/.test(foo) yang artinya kita ingin memeriksa apakah kata "Belajar" ada di dalam string foo. Terlihat kita dapat langsung memanggil method RegExp dari penulisan literal, tanpa harus menyimpanya kedalam variabel terlebih dahulu.
    ■ Perintah terakhir /belajar/.test(foo) hasilnya false karena perbedaan huruf kecil di karakter "b". Artinya kata "belajar" tidak ditemukan (bersifat case sensitif).
__________________________________________________________________________________
  ■ Method RegExp.prototype.exec()
  Method exec() berfungsi untuk mencari karakter atau kata yang cocok dengan pola regular expression, kemudian menyimpan hasilnya ke dalam array.

  ■ Berikut contoh penggunaannya:
    var foo = "1 jam sama dengan 60 menit, juga sama dengan 3600 detik";
    var pola = /\d+/;

    console.log(pola.exec(foo)); // Array ["1"]

    Pola \d+ artinya cari karakter angka dengan jumlah digit 1 atau lebih. Sehingga perintah pola.exec(foo) digunakan mencari karakter angka dari string foo. Hasilnya adalah angka 1 yang menjadi element array. Ini merupakan fitur default dari method exec(), yakni ketika sebuah pola yang cocok sudah ketemu, method akan langsung berhenti.

    ■ Bagaimana cara mencari "semua" digit? Kita bisa menambahkan sebuah flag g atau penanda di dalam pola regular expression. Pola tersebut menjadi seperti ini:

    var foo = "1 jam sama dengan 60 menit, juga sama dengan 3600 detik";
    var pola = /\d+/g;

    consloe.log(pola.exec(foo)); // Array ["1"]
    console.log(pola.exec(foo)); // Array ["60"]
    console.log(pola.exec(foo)); // Array ["3600"]
    console.log(pola.exec(foo)); // null

    Setiap kali method exec() dipanggil, pencarian pola akan lanjut ke posisi berikutnya. Jika tidak adalagi pola yang cocok, method ini akan mengembalikan nilai null.

    Oleh karena itu fitur method exec() yang seperti ini untuk mencari seluruh pola, kita harus menggunakan perulangan. Konsepnya, selama method pola.exec(foo) belum mengembalikan nilai null, lakukan terus pencarian pola.
__________________________________________________________________________________
■ Pola Reguler Expression
Mempelajari pola reguler expression bisa dibilang "gampang-gampang susah". Karakter penyusun pola regexp tidak begitu banyak, tapi hasil dari pola yang ditulis cukup susah untuk dibaca. Agar mudah dipahami, kita akan banyak menggunakan contoh kode program.
  ■ Pola RegExp Sebagai String
  Mari kita mulai dari pola yang paling sederhana yakni jika isi regular expression berbentuk string biasa yang terdiri dari sebuah kata atau berberapa karakter. Jika ditulis seperti ini, pola tersebut akan cocok selama di dalam string terdapat kata tersebut (di posisi mana saja).
  ■ Berikut contohnya:

    var foo = "Belajar JavaScript";

    console.log(/JavaScript/.test(foo)); // true
    console.log(/javaScript/.test(foo)); // false
    console.log(/Belajar/.test(foo)); // true
    console.log(/belajar/.test(foo)); // false
    console.log(/Java/.test(foo)); // true
    console.log(/ajar/.test(foo)); // true

    ■ Disini kita memiliki sebuah string "Belajar JavaScript" yang disimpan ke dalam variabel foo. Perhatikan penulisan pola regular expression, semuanya berisi kata-kata biasa. Method test() akan menghasilkan nilai true jika kata tersebut ada di dalam string foo.
__________________________________________________________________________________
■ Pola Character Set
Pola selanjutnya adalah character set, dimana kita bisa membuat syarat bahwa hanya karakter tertentu saja yang boleh ditulis. Ini dibuat menggunakan tanda kurung siku: [ dan ]. Hanya karakter yang ada di dalam tanda kurung ini saja yang akan memenuhi syarat.

  var pola = /[abcde]../;

  console.log(pola.test("abaa")); // true
  console.log(pola.test("fba")); // false
  console.log(pola.test("1dd")); // false
  console.log(pola.test("add")); // true
  console.log(pola.test(" dd")); // false
  console.log(pola.test("belajar")); // true

  ■ Pola /[abcde]../ artinya, digit pertama hanya bisa diisi oleh salah satu dari huruf a, b, c, d atau e. Kemudian salah satu huruf tersebut diikuti setidaknya oleh 2 karakter lain (bebas mau karakter apa saja).
  ■ Dengan demikian, string yang memenuhi syarat ini adalah: "abaa", "add" dan "belajar". String "fba" menjadi false karena digit pertama diawali huruf f. String "1dd" juga false karena karakter pertama berupa angka, sedangkan string " dd" hasilnya false karena karakter pertama berisi spasi. Pola /[abcde]../ bisa juga ditulis menjadi: /[a-e]../.