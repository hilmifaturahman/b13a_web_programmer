■ HTML kepanjangan dari Hypertext Markup Language, artinya adalah bahasa markup(penanda) berbasis teks atau bisa disebut sebagai formatting language(bahasa untuk memformat). Nantinya akan di tampilkan melalui halaman web pada web browser.
__________________________________________________________________________________
■ Untuk melihat kode HTML pada web browser bisa menggunakan inspect element dengan klik kanan pada web browser klik ispect element atau bisa tekan F12.
__________________________________________________________________________________
■ Tag HTML ada memiliki tag pembuka <namatag> dan tag penutup</namatag>
__________________________________________________________________________________
■ Format tag pada HTML:
  <namatag atribut="nilai atribut">Isi yang akan di format</namatag>
__________________________________________________________________________________
■ Struktur dasar file HTML:
  <!DOCTYPE html>
  <html>
    <head>
        <title>Judul File HTML</title>
    </head>
    <body>
        Website <strong><em>Pertama</em></strong> Saya
    </body>
  </html>
  ■ <!DOCTYPE HTML>
  Adalah Tag awal dari setiap dokumen HTML, tag ini berfungsi untuk menginformasikan pada browser bahwa dokumen yang sedang dibuka adalah dokumen HTML. Tag ini perlu dicantumkan disetiap dokumen HTML yang akan anda buat.
  ■ <HTML> ... </HTML>
  Awal dari isi dokumen HTML dimulai dari sini, semua kode HTML yang akan anda buat akan ditulis di dalam tag ini, perhatikan juga bahwa setiap tag harus memiliki tag penutup.
  ■ <head> ... <head>
  Tag Head akan digunakan untuk menyimpan berbagai informasi tentang dokumen HTML. Apa yang terdapat di dalam tag ini, tidak akan ditampilkan secara langsung pada web browser.
  ■ <title> ... </title>
  Salah satu contoh informasi yang terdapat di dalam tag Head adalah title. Title akan menampilkan teks pada judul browser atau pada tab browser.
  ■ <body> ... </body>
  Apa yang ingin anda tampilkan pada browser akan ditulis di dalam tag ini, tag body merupakan tag pembuka dari badan dokumen HTML.
__________________________________________________________________________________
■ Memuat gambar
  <img>
  ■ Tag img tidak memliki tag penutup atau disebut Self Close Tag. Sebagai penggantinya bisa tambahkan tanda slash(/) sebelum tutup kurung(>).
  ■ Setiap tag img, selain memiliki atribut src untuk menyimpan lokasi gambar, ada juga atribut alt yang akan digunakan sebagai teks alternatif ketika gambar tidak berhasil dimuat atau gambar hilang.
    <img src="gambar.jpg alt="gambar"/>
  ■ Dan atribut lainnya adalah atribut width dan height, yang berfungsi untuk menentukan lebar dan tinggi dari gambar tersebut. Memang hal ini tidak perlu dilakukan karena gambar secara otomatis akan terload dengan ukuran sebenarnya, namun hal ini sangat dianjurkan untuk mempercepat proses pemuatan gambar.
    <img src="gambar.jpg alt="gambar" width="100px" height="100px"/>
__________________________________________________________________________________
■ Membuat link
  <a>link</a>
  ■ Link ini akan membuat konten atau elemen HTML dapat di klik dan akan mengarahkan/membawa ke halaman web lainnya. Biasanya suatu link ditampilkan berwarna biru dan bergaris bawah (selama belum diberi style).
  ■ Link atau biasa disebut dengan anchor (pengait) dapat dibuat dengan menambahkan tag <a> pada teks yang ingin kita buat menjadi link.
  ■ Perlu ada penambahan atribut href untuk menjadi sebuah link
    Klik <a href="http://www.alamat-tujuan.com">disini</a> untuk mendownload
__________________________________________________________________________________
■ Heading atau penjudulan
  <h1></h1> sampai <h6></h6>
  ■ Tag h1 sampai h6 digunakan untuk membuat judul, tag h1 ukuran paling besar dan h6 ukuran paling kecil, h2 sampai h6 bisa di gunakan sebagai sub judul.
__________________________________________________________________________________
■ Draw io online / sketsa
  https://app.diagrams.net/
__________________________________________________________________________________
■ Membuat list atau daftar
  ■ Ordered list(menggunakan penomoran)
    <ol>
      <li>list 1</li>
      <li>list 2</li>
    <ol/>
  ■ Unordered list(menggunakan simbol)
    <ul>
      <li>list ■</li>
      <li>list ■</li>
    </ul>
  ■ Nested list(list di dalam list)
    <ol>
      <li>list 1
        <ul>
          <li>list ■</li>
          <li>list ■</li>
        </ul>
      </li>
      <li>list 2
        <ul>
          <li>list ■</li>
          <li>list ■</li>
        </ul>
      </li>
    <ol/>
__________________________________________________________________________________
■ div atau division(pembagian)
  <div></div>
  ■ Tag div hanya digunakan untuk membuat dokumen HTML lebih terstruktur dengan membagi-bagi dokumen ke dalam bagian-bagian yang lebih spesifik.
  ■ Tag div bisa di tambahkan atribut id atau class sebagai penamaan dan nanti bisa menjadi selector di CSS.
  ■ Pada halaman web biasanya ada beberapa bagian seperti berikut:
    ■ header adalah bagian kepala website berisi logo, nama, slogan, menu website dll.
    ■ content berisi isi dari website itu sendiri.
    ■ sidebar berada disamping content bisaya berisi iklan, kategori artikel widget atau hiasan lainnya.
    ■ footer bagian kaki website, biasa berisi Copyrigth 2023 by someone, atau bisa berisi lainnya.
  ■ contoh penggunaan div:
    <div id="header">isi header
    </div>
    <div id="content">isi content
    </div>
  ■ atribut id digunakan untuk penamaan element HTML yang memiliki karakteristik unik/berbeda. Tidak boleh ada dua atau lebih element yang mempunyai id yang sama.
  ■ atribut class digunakan untuk penamaan element yang memiliki karakteristik atau struktur sama dan dapat digunakan berulang kali dalam HTML.
__________________________________________________________________________________
■ <div id="wrapper">
    <div id="content">
        <div id="article"></div>
        <div id="sidebar"></div>
    </div>
  </div>
  ■ <div id="wrapper"> adalah parent yang di dalam nya di sebut child <div id="content">
  ■ <div id="content"> adalah parent yang didalamnya ada child <div id="article"> dan <div id="sidebar">
  ■ <div id="article"> memiliki hubungan sibling atau saudara dengan <div id="sidebar">
__________________________________________________________________________________
■ Form
  ■ Dalam sebuah website biasanya terdapat satu atau lebih form, seperti form pencarian, registrasi dan lain sebagainya. Form ini biasa digunakan untuk mengumpulkan data dari pengunjung website.
    <form>
       <h1>Formulir Pendaftaran</h1>
       ...
    </form>
  ■ Perlu adanya kontrol dalam tag form diantaranya:
    ■ label
      ■ Label digunakan untuk memberikan keterangan pada setiap input yang ada      
      ■ Atribut for diisi dengan isi dari atribut name pada kontrol yang ingin diberi label
        <label for="name">Keterangan Input</label>
    ■ text
      ■ Control input ini dapat diisi dengan teks yang memiliki kata yang tidak terlalu panjang/hanya satu baris, biasa digunakan dalam form pencarian, nama dan lain sebagainya.
        <input type="text" name="nama" />
      ■ bisa ditambahkan atribut value jika ingin terisi otomatis
        <input type="text" name="nama" value="Hacktiv8"/>
      ■ bisa ditambah atribut placeholder sebagai contoh isi dalam input
        <input type="text" name="nama" placeholder="masukkan nama"/>
      ■ atribut required agar input wajib diisi(ketika kosong akan ada peringatan) 
        <input type="text" name="nama" placeholder="masukkan nama" required/>
    ■ text area    
      ■ Sama halnya dengan Input Text, namun textarea dapat diisi lebih dari satu baris, cocok digunakan untuk isian yang panjang, seperti alamat, deskripsi, atau biodata.
      ■ text area menggunakan tag <textarea></textarea>
        <textarea name="alamat" placeholder="masukkan alamat" required></textarea>
    ■ combo box
      ■ Combo Box adalah kontrol yang memiliki pilihan ketika diklik. Pembuatannya sama seperti pembuatan Daftar/List namun dengan tag yang berbeda.
        <select name="kota">
          <option>Jakarta</option>
          <option>Bandung</option>
          <option>Tasikmalaya</option>
        </select>
    ■ submit/button
      ■ Submit atau Button, berupa tombol yang dapat di klik. Penggunaan atribut value pada kontrol ini akan merubah text yang ada di dalamnya.
        <input type="submit" value="kirimkan data">
__________________________________________________________________________________
■ Jika ingin load cdn bootstrap untuk template
  https://getbootstrap.com/docs/4.3/getting-started/introduction/
__________________________________________________________________________________
■ tabel
  ■ untuk membuat data dengan tabel di HTML bisa menggunakan tag table
    <table></table>
  ■ untuk membuat baris gunakan tag tr singkatan dari table row (ditulis di dalam tag table)
    <table>
      <tr></tr>
    </table>
  ■ untuk menentukan banyaknya kolom, tergantung dari banyaknya tag <td>(table data) yang digunakan di dalam tag <tr>
    <table>
        <tr>
            <td>No</td>
            <td>Nama</td>
            <td>Alamat</td>
        </tr>
    </table>
  ■ Untuk menyatukan kolom atau baris (merge-cell) kita tambahkan atribut colspan (untuk merge secara horizontal) atau rowspan (untuk merge vertically).
  ■ untuk menampilkan garis pada tabel tambahkan atribut border dalam tag tabel
    <table border="1">
        <thead>
            <tr>
                <td rowspan="2">No</td>
                <td colspan="2">Jenis Kelamin</td>
                <td rowspan="2">Nama</td>
            </tr>
            <tr>
                <td>L</td>
                <td>P</td>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>L</td>
                <td></td>
                <td>Hacktiv8</td>
            </tr>
            <tr>
                <td>2</td>
                <td></td>
                <td>P</td>
                <td>Gita</td>
            </tr>
            <tr>
                <td>3</td>
                <td>L</td>
                <td></td>
                <td>Arif</td>
            </tr>
        </tbody>
    </table>
  ■ <thead></thead> untuk bagian judul tabel
  ■ <tbody></tbody> untuk bagian isi tabel
  ■ <tfoot></tfoot> untuk bagian footer tabel
__________________________________________________________________________________
■ inline dan block
  ■ inline tidak memakan baris baru dan hanya memiliki lebar sepanjang yang di butuhkan sesuai dengan kontennya. contoh element dengan sifat inline: span, b, i.
  ■ block kebalikan dari inline selalu memakan baris baru dan memiliki ukuran lebar full satu halaman, contoh element dengan sifat block: div, h1, h2.
