■ Javascript adalah Bahasa pemrograman yang digunakan untuk membuat sebuah halaman web menjadi interaktif.
■ JavaScript berjalan atau beroperasi di browser yang ada di tiap komputer yang digunakan oleh visitor atau user web kita.
■ Javascript awalnya bernama Mocha, lalu berubah menjadi LiveScript saat browser Netscape Navigator 2.0 rilis versi beta (September 1995). Namun, setelah itu dinamai ulang menjadi Javascript.
■ JavaScript berbeda dengan HTML, dimana JavaScript bersifat dinamis, dimana banyak proses yang akan berjalan seiring  program JavaScript ini berfungsi.
■ Apakah JavaScript menggantikan HTML? Tidak!

■ Penggunaan Javascript
  ■ Internal
    ■ Cara yang umum yang dipakai adalah menuliskanya dalam tag <script>. Tag <script> bisa dibuat di dalam tag <head>, maupun di dalam tag <body>. Contoh:

    <!DOCTYPE html>
    <html>
    <head>
        <meta charset="utf-8">
        <title>Cara Penulisan Javascript</title>
        <script>
        console.log("Hi, ini kode Javascript");
        </script>
    </head>
    <body>
    <!-- Isi konten -->
    <script>
    documeent.write("Saya mulai belajar Javascript!");
    </script>
    </body>
    </html>

  ■ File External
    ■ Kita bisa menuliskannya pada file terpisah. Caranya, buatlah sebuah file yang berekstensi .js, misalnya isinya sebagai berikut.

    filename:alert.js:

    alert("Saya memanggil Javascript melalui alert.js")

    panggil di HTML
    <!DOCTYPE html>
    <html>
    <head>
        <title>Panggil external Javascript</title>
        <script =src"alert.js"></script>
    </head>
    <body>
        <!-- Isi konten -->
    </body>
    </html>


■ Variabel
  ■ Variabel adalah suatu penyimpanan untuk data dan kita dapat menggunakan variabel untuk menyimpan beberapa informasi atau data.

  ■ Untuk membuat sebuah variabel pada JavaScript, kita dapat menggunakan keyword var, let atau const.

  ■ Statement berikut adalah untuk membuat (mendeklarasikan) variabel dengan nama "pesan":

  <!DOCTYPE html>
  <html>
    <head>
      <title>Penggunaan Variable di JS</title>
    </head>
    <body>
      <h1>Penggunaan Variable di JS</h1>

      <div id="nama"></div>
      <div id="lokasi"></div>

      <script>
        var nama = "Workshop 4 Days;
        var lokasi = "Online";

        document.getElementByID("nama").innerHTML = nama;
        document.getElementByID("lokasi").innerHTML = lokasi;
      </script> 
    </body>
  </html>

■ Tipe Data
  ■ Tipe data adalah jenis-jenis data yang bisa kita simpan di dalam variabel.
  ■ Javascript adalah bahasa yang bersifat dynamic typing, artinya kita tidak harus menuliskan tipe data pada saat pembuatan variabel seperti pada bahasa C, C++, Java, dsb. yang bersifat static typing.
  ■ Ada beberapa tipe data dalam pemrograman Javascript:
    ■ Integer atau Number (bilangan bulat) 
    ■ String (teks)
    ■ Boolean
    ■ Object
  ■ Tipe Data Number
  <!DOCTYPE html>
  <html>
    <head>
      <title>Tipe Data Number di JS</title>
    </head>
    <body>
      <h1>Tipe Data Number di JS</h1>
      <div id="hasil"></div>

      <script>
        var angka = 80;

        document.getElementByID("hasil").innerHTML = angka;
      </script>
    </body>
  </html>

  ■ Tipe Data String
  <!DOCTYPE html>
  <html>
    <head>
      <title>Tipe Data String di JS</title>
    </head>
    <body>
      <h1>Type Data String di JS</h1>

      <div id="hasil"></div>

      <script>
        var kalimat = "Belajar JS di Workshop WFDF";

        document.getElementByID("hasil").innerHTML = kalimat;
      </script>
    </body>
  </html>

  ■ Tipe data Array
  <!DOCTYPE html>
  <html>
    <head>
      <title>Tipe Data Array di JS</title>
    </head>
    <body>
      <h1>Tipe Data Array di JS</h1>

      <div id="hasil"></div>
      <script>
        var transport = ["Mobil", "Motor", "Pesawat", "Kapal"];

        document.getElementByID("hasil").innerHTML = transport[1];
        document.getElementByID("hasil").innerHTML = transport[3];

      </script>
    </body>  
  </html>

  ■ Tipe Data Object
  <!DOCTYPE html>
  <html>
    <head>
      <title>Tipe Data Objek di JS</title>
    </head>
    <body>
      <h1>Tipe Data Object di JS</h1>

      div id="hasil"></div>

      <script>
        var manusia = {
            nama : "Hilmi",
            asal : "Sukabumi",
            usia : 25,
        };
      
      
        document.getElementByID("hasil").innerHTML = manusia.nama + "tinggal di" + manusia.asal;

      </script>    
    </body>
  </html>

■ Operator Aritmatika
  ■ Operator aritmatika merupakan operator untuk melakukan operasi aritmatika seperti penjumlahan, pengurangan, pembagian, perkalian, dsb.
  ■ Operator aritmatika terdiri dari:
    1. Penjumlahan(+) menjumlahkan 2 operand
    2. Pengurangan(-) mengurangi suatu operand dengan operan yang lainnya
    3. Perkalian(*) mengalikan suatu operand dengan operan yang lainnya
    4. Pembagian(/) operasi pembagian suatu operand akan dibagi dengan operand lainnya
    5. modulus(%) menghasilkan sisa bagi dari hasil pembagian suatu operand dengan operand lainnya
    6. Increment(++) menambah 1 nilai keatas pada operand/variable
    7. Decrement(--) mengurangi 1 nilai kebawah pada operand/variable

  <!DOCTYPE html>
  <html>
    <head>
      <title>Penggunaan Operator Aritmatika di JS</title>
    </head>
    <body>
      <h1>Penggunaan Operator Aritmatika di JS</h1>

      <div id="penjumlahan"></div>
      <div id="pengurangan"></div>
      <div id="perkalian"></div>
      <div id="pembagian"></div>
      <div id="modulus"></div>

      <script>
        var bilangan1 = 6;
        var bilangan2 = 2;

        var penjumlahan = bilangan1 + bilangan2;
        var pengurangan = bilangan1 - bilangan2;
        var perkalian = bilangan1 * bilangan2;
        var pembagian = bilangan1 / bilangan2;
        var modulus = bilangan1 % bilangan2;

        document.getElementByID("penjumlahan").innerHTML = penjumlahan;
        document.getElementByID("pengurangan").innerHTML = pengurangan;
        document.getElementByID("perkalian").innerHTML = perkalian;
        document.getElementByID("pembagian").innerHTML = pembagian;
        document.getElementByID("modulus").innerHTML = modulus;
      </script>
    </body>
  </html>

■ Function
  ■ Function adalah sub-program yang bisa digunakan kembali baik di dalam program itu sendiri, maupun di program yang lain.

  ■ Fungsi didalam Javascript adalah sebuah objek. Karena memiliki properti dan juga method.

  function namaFungsi(){
    console.log("Hello World!");
  }

  <!DOCTYPE html>
  <html>
  <head>