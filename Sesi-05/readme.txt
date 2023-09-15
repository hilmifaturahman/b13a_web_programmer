■ Javascript adalah Bahasa pemrograman yang digunakan untuk membuat sebuah halaman web menjadi interaktif.
■ JavaScript berjalan atau beroperasi di browser yang ada di tiap komputer yang digunakan oleh visitor atau user web kita.
■ Javascript awalnya bernama Mocha, lalu berubah menjadi LiveScript saat browser Netscape Navigator 2.0 rilis versi beta (September 1995). Namun, setelah itu dinamai ulang menjadi Javascript.
■ JavaScript berbeda dengan HTML, dimana JavaScript bersifat dinamis, dimana banyak proses yang akan berjalan seiring  program JavaScript ini berfungsi.
■ Apakah JavaScript menggantikan HTML? Tidak!
__________________________________________________________________________________
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
__________________________________________________________________________________
  ■ File External
    ■ Kita bisa menuliskannya pada file terpisah. Caranya, buatlah sebuah file yang berekstensi .js, misalnya isinya sebagai berikut.
    ■ filename:alert.js:
    alert("Saya memanggil Javascript melalui alert.js")

    ■ panggil di HTML
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
__________________________________________________________________________________
■ Variabel
  ■ Variabel adalah suatu penyimpanan untuk data dan kita dapat menggunakan variabel untuk menyimpan beberapa informasi atau data.
  ■ Untuk membuat sebuah variabel pada JavaScript, kita dapat menggunakan keyword var, let atau const.
__________________________________________________________________________________
  ■ Contoh penggunaan var:
  function contohVar() {
    var x = 10;
    if (true) {
      var x = 20;
      console.log(x); // Output: 20
    }
    console.log(x); // Output: 20
  }
  contohVar();

    ■ Dalam contoh ini, variabel x dideklarasikan dengan var di dalam fungsi contohVar(). Meskipun x dideklarasikan kembali di dalam blok if, perubahan tersebut berlaku di seluruh fungsi karena variabel var memiliki lingkup fungsi.
  ■ Contoh penggunaan let:
  function contohLet() {
    let y = 10;
    if (true) {
      let y = 20;
      console.log(y); // Output: 20
  }
    console.log(y); // Output: 10
  }
  contohLet();
    ■ Dalam contoh ini, variabel y dideklarasikan dengan let di dalam fungsi contohLet(). Ketika y dideklarasikan kembali di dalam blok if, perubahan tersebut hanya berlaku di dalam blok itu sendiri. Di luar blok, variabel y tetap memiliki nilai awalnya.
  ■ Contoh penggunaan const:
  function contohConst() {
    const z = 10;
    if (true) {
      const z = 20;
      console.log(z); // Output: 20
    }
    console.log(z); // Output: 10
  }
  contohConst();
    ■ Dalam contoh ini, variable z dideklarasikan dengan const di dalam fungsi contohConst(). Meskipun z dideklarasikan kembali di dalam blok if, perubahan tersebut hanya berlaku di dalam blok itu sendiri. Konstanta z di luar blok tetap memiliki nilai awalnya dan tidak dapat diubah.
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
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
__________________________________________________________________________________
■ Function
  ■ Function adalah sub-program yang bisa digunakan kembali baik di dalam program itu sendiri, maupun di program yang lain.
  ■ Fungsi didalam Javascript adalah sebuah objek. Karena memiliki properti dan juga method.
__________________________________________________________________________________
  function namaFungsi(){
    console.log("Hello World!");
  }
__________________________________________________________________________________
  <!DOCTYPE html>
  <html>
  <head>
    <title>Membuat Function di Javascript</title>
  </head>
  <body>
    <h1>Membuat Function di Javascript</h1>
    <h2>www.hacktiv8.com</h2>

    <!-- id hasil-->
    <div id="hasil"></div>

    <script>
      // membuat function tampilkaan Nama
      function tampilkan_nama(){
        return "Hacktiv8 Front End Web Development"
      }

      document.getElementByID("hasil").innerHTML = tampilkan_nama();    
    </script>
  </body>
  </html>
__________________________________________________________________________________
■ Event
  ■ Event pada Javascript adalah bagian dari element HTML berisi serangkaian event yang dapat memicu Javascript.
  ■ Berikut beberapa event yang ada pada javascript:
    ■ onchange = An HTML element has been changed
    ■ onclick = The use clicks an HTML element
    ■ onmouseover = The user moves the mouse over an HTML element
    ■ onmouseout = The user moves the mouse away from an HTML element
    ■ onkeydown = The user pushes a keyboard key
    ■ onload = The browser has finished loading the page
__________________________________________________________________________________
  ■ onclick adalah suatu kejadian yang terjadi ketika sebuah html di klik.
  <!DOCTYPE html>
  <html>
  <head>
    <title>Mengenal Event pada JavaScript</title>
  </head>
  <body>
    <h1>Mengenal Event Pada Javascript</h1>
    <h2>www.hacktiv8.com</h2>

    <!-- memberikan event pada element tombol -->
    <button onclick="tampilkan_nama()">KLIK SAYA</button>

    <!-- id hasil-->
    <div id="hasil"></div>

    <script>
      // membuat function tampilkan nama
      function tampilkan nama(){
        document.getElementByID("hasil").innerHTML = "<h3>Nama Saya adalah Fox</h3>;
      }

    <script/>
  </body
  </html>
__________________________________________________________________________________
■ Javascript Output
  ■ menggunakan fungsi console.log
    ■ fungsi console.log() adalah fungsi untuk menampilkan teks ke console javascript.
    ■ fungsi console.log() biasanya digunakan untuk debugging. Karena setiap pesan error di javascript selalu di tampilkan di console.
  ■ menggunakan fungsi alert()
    ■  fungsi alert() adalah fungsi untuk menampilkan jendela dialog. Fungsi sebenarnya berada pada objek window.
  ■ menggunakan document.write()
    ■ Objek document adalah objek yang mewakili dokumen HTML di dalam javascript.
    ■ Dalam objek document, terdapat fungsi write() untuk menulis sesuatu ke dokument HTML.
    ■ Selain fungsi write(), objek document juga menyediakan berbagai macam fungsi untuk manipulasi dokumen HTML.
__________________________________________________________________________________
■ Ada tiga macam jendela dialog pada javascript:
  ■ Jendela dialog alert();
    ■ dialog alert() biasanya di gunakan untuk menampilkan sebuah pesan peringatan atau informasi.
    ■ fungsi alert() berada dalam objek windows.
    ■ karena objek window bersifat global, kita boleh tidak menulisnya.
    ■ Dialog alert() tidak akan mengembalikan nilai apa-apa saat dieksekusi.
  ■ Jendela dialog comfirm();
    ■ Dialog confirm() digunakan untuk melakukan konfirmasi dalam melakukan tindakan tertentu.
    Misalnya:
    saat kita menghapus sesuatu, maka ada baiknya menampilkan dialog confirm().
    karena tindakan tersebut cukup bahaya.
    dialog confirm() akan mengembalikan nilai true apabila kita memilih tombol OK dan akan mengembalikan nilai false apabila kita memilih Cancel.
    Nilai kembalian ini dapat kita tampung dalam variable untuk diproses.
  ■ Jendela dialog prompt();
    ■ dialog prompt() berfungsi untuk mengambil sebuah inputan dari pengguna.
    ■ dialog prompt() akan mengembalikan sebuah nilai string dari apa yang diinputkan oleh pengguna.
    ■ dialog prompt() memiliki beberapa parameter yang harus diberikan:
      ■  teks yang akan ditampilkan di form;
      ■  nilai default untuk field input.
      pada contoh di atas, kita memberikan nilai defaultnya berupa string kosong dengan tanda petik "".
■ Kapan waktu yang tepat menggunakan alert, confirm dan prompt
  ■ Saat kita hanya ingin menampilkan informasi saja, maka gunakan alert()
  ■ saat kita ingin jawaban konfirmasi pengguna, maka gunakan confirm()
  ■ dan apabila kita ingin mengambil data teks dari pengguna, maka gunakan prompt().
__________________________________________________________________________________
■ Function & events
  ■ Sebelum membuat kode, kita selalu harus mulai dari apa masalahnya. Masalah ini dipecah menjadi 3 bagian: input, proses, output. Input dan output selalu perlu kita tentukan terlebih dahulu. Aopa input dari masalah ini. Apa output yang diinginkan?
  ■ Contohnya , masalahnya adalah untuk menghitung grade seorang murid. input nilai seorang murid dalam bentuk angaka (0-100), output adalah grade murid tersebut(A, B, C, D, E). Setelah mengetahui jenis input dan output yang diinginkan, kita mulai membuat proses perubahan input tersebut jadi output.
  ■ Setelah menjadi kode, tentu kita mau memakainya berkali-kali. Program yang di buat tujuannya memudahkan dan membuat suatu proses yang tadinya manual jadi lebih otomatis. Tapi bagaimana caranya code tersebut bisa dipanggi berkali-kali. Mirip seperti memberi nama ke seseorang agar mudah di panggil.
  ■ Masih menggunakan contoh mengubah nilai (0-100) menjadi grade (A-E), kita buat sebuah function yang menerima input nilai, dan memberi output grade
__________________________________________________________________________________
function hitungGrade (nilai) {
  let grade = ""
  if (nilai >= 90) {
    grade = "A"
  } else if (nilai >= 80) {
    grade = "B"
  } else if (nilai >= 70) {
    grade = "C"
  } else if (nilai >= 60) {
    grade = "D"
  } else
    grade = "E"
  return grade
}
__________________________________________________________________________________
■ perhatikan untuk membuat function kita tulis dulu keyword function, lalu nama yang diberikan, lalu kurung biasa yang berisi input, diikuti kurung kurawal tempat semua kode yang mau kita gunakan untuk proses dan output didalam. keyword return digunakan untuk mengembalikan output. Tetapi jika kita memerlukannya untuk sebuah HTML, outputnya perlu di cocokkan jadi format HTML.
__________________________________________________________________________________
■ Web yang pasif(hanya di baca)tidak semenarik yang interaktif. Tapi untuk membuat web(HTML) interaktif, perlu ada sesuatu yang terjadi. Event adalah saat sesuatu terjadi: klik, mouse lewat, mouse keluar, ketikan di kontak input, klik di lepas, dan lain-lain. Semua event itu bisa kita buatkan menyambung dengan function.
__________________________________________________________________________________
■ Bagaimana cara membuat event? dari file HTML, di sebuah element/tag HTML, kita tambahkan attribute event tersebut.

<html>
  <head>
    <title>Belajar Event</title>
  </head>

  <body
    <button>Klik aku</button>
  </body>
</html>
__________________________________________________________________________________
■ Misalkan di html diatas, kita tambahkan event klik di buttonnya, saat button di klik, function ubahText akan di jalankan

  <button onclik="ubahText()">Klik aku</button>
__________________________________________________________________________________
■ Perlu kita tentukan juga function ubahText melakukan apa. Tambahkan tag script untuk membuat function langsung di file HTML yang sama. Bisa juga tag script untuk menghubungkan function yang ada di file javascript terpisan(js).

<body
  <button onclick="ubahText">Klik aku</button>
  <script>
    function ubahText() {

    }
   </script>
</body>
__________________________________________________________________________________
<body>
  <button onclick="ubahText()">Klik aku</button>
  <script src="file.js"></script>
</body>
__________________________________________________________________________________
<body>
  <button id="tombol" onclick="ubahText()">Klik aku</button>
  <script>
    function ubahText() {
      document.getElementByID("tombol").innerHTML = "Halo YAL"
    }
  </script>
</body>
__________________________________________________________________________________
■ hitung Mundur Maju
	<body>
		<h1>Hitung Mundur Maju:</h1>
		<button onclick="mundur()">mundur</button>
		<button onclick="maju()">maju</button>
		<p id="hasil"></p>
	</body>
	<script>
		var nilai_awal = 10;
		var nilai_akhir = document.getElementById("hasil");

		function mundur() {
			nilai_awal--;
			nilai_akhir.innerHTML = nilai_awal;
		}

		function maju() {
			nilai_awal++;
			nilai_akhir.innerHTML = nilai_awal;
		}
__________________________________________________________________________________
■ Javascript Conditional
  ■ let kondisi = true
    if (kondisi) {
    // ini didalam blok kode if
    }
    // ini diluar blok kode if
  ■ let kondisi = "lapar"
    if (kondisi === "lapar"){
      // waktu makan
    }
    if (kondisi === "tidak lapar"){
      // bukan waktu makan
    }
  ■ let kondisi = "lapar"
    if (kondisi === "lapar"){
       // waktu makan
    } else {
      // bukan waktu makan
    }
  ■ <!DOCTYPE html>
    <html>  
    <head>
      <title>Belajar kondisional</title>
    </head>
    <body>
      <button onclick="ceklapar()">Cek Lapar</button>
      <p id="hasil"></p>
       
      <script>
        function ceklapar() {
          let kondisi = "lapar"
          if (kondisi === "lapar") {
            //waktu makan
            hasil = "waktu makan"
          } else {
            // bukan waktu makan
            hasil = "bukan waktu makan"
          }
          document.getElementById("hasil").innerHTML = hasil
        }
      </script>
    </body>
    </html>
    ■ Note: saat ini button nya tidak menerima input dari kita, jadi mengubah kondisi "lapar" atau tidaknya kita perlu edit file, save dan refresh lagi.
__________________________________________________________________________________
  ■ Sekarang kita buat versi dimana kita pakai textbox untuk menerima input kondisi "lapar" atau tidak.
    <!DOCTYPE html>
    <html>
    
    <head>
      <title>Belajar kondisional</title>
    </head>
    <body>
      <label>Kondisi:</label><input id="kondisi" type="text"><br><br>
      <button onclick="ceklapar()">Cek Lapar</button>
      <p id="hasil"></p>
       
      <script>
        function ceklapar() {
          let kondisi = document.getElementById("kondisi").value
          let hasil = ""
          if (kondisi === "lapar") {
            //waktu makan
            hasil = "waktu makan"
          } else {
            // bukan waktu makan
            hasil = "bukan waktu makan"
          }
          document.getElementById("hasil").innerHTML = hasil
        }
      </script>
    </body>
    </html>
__________________________________________________________________________________
  ■ Lalu bagaimana dengan kondisi yang ada diantara lapar atau tidak? Kita bisa membuat lebih dari 2 pilihan dengan menambahkan else if

  let kondisi = "lapar"
  if (kondisi === "lapar"){
    // waktu makan
  } else if(kondisi === "kenyang") {
    // bukan waktu makan
  } else {
    // boleh ngemil
  }
__________________________________________________________________________________
  ■ jumlah else if tidak terbatas tergantung kebutuhan.
__________________________________________________________________________________
■ while loop
let hitung = 0
while(hitung > 1000) {
  // ini di dalam perulangan
  hitung = hitung + 1
}
__________________________________________________________________________________
<!DOCTYPE html>
<html>
<head>
  <title>Belajar perulangan</title>
</head>
<body>
  <button onclick ="print()">Print 1000x</button>
  div id="text"></div>
  <script>
    function print() {
      const dt = document.getElementById("text")
      let hitung = 0
      while (hitung < 1000) {
        //ini didalam perulangan
        dt.innerHTML = dt.innerHTML + "<p>Saya tidak akan terlambat lagi</p>"
        hitung = hitung + 1
      }
    }
  </script>
</body>
</html>
__________________________________________________________________________________
■ for loop
for (let hitung = 0; hitung < 3; hitung = hitung + 1){
}
__________________________________________________________________________________
<!DOCTYPE html>
<html>
<head>
  <title>Belajar perulangan</title>
</head>
<body>
  <button onclick ="print()">Print 3x</button>
  div id="text"></div>
  <script>
    functin print() {
      const dt = document.getElementById("text")
      let hitung = 0
      for (let hitung = 0; hitung < 3; hitung = hitung + 1) {
        //ini didalam perulangan
        dt.innerHTML = dt.innerHTML + "<p>Saya sudah belajar for loop</p>"
      }
    }
  </script>
</body>
</html>
__________________________________________________________________________________
■ menampilkan array dengan pengulangan
<!DOCTYPE html>
<html>
<head>
  <title>Belajar perulangan</title>
</head>
<body>
  <button onclick ="print()">Print Makanan Kesukaan</button>
  <ul id="list"></ul>
  <script>
    functin print() {
      const dt = document.getElementById("list")
      const list_makanan = ["Nasi Goreng", "Mie Goreng", "Ayam Bakar"]
      for (let index = 0; index < list_makanan.length; index = index + 1) {
        dt.innerHTML = dt.innerHTML `<li>${list_makanan[index]}</li>`
      }
    }
  </script>
</body>
</html>
