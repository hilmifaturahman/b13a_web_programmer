■ CSS adalah singkatan dari Cascading Styling Sheet
■ CSS adalah Bahasa style yang digunakan untuk mempercantik atau memperindah tampilan elemen pada HTML web seperti format, warna, posisi dan lain sebagainya.
■ Dengan CSS, file HTML hanya digunakan untuk konten. Seluruh bentuk styling tampilannya di atur di files CSS, misalnya mengubah jenis teks atau font, warna, background, border, format tulisan, dan berbagai efek lainnya.
__________________________________________________________________________________
■ Format CSS:
  selector {
    property: value;
  }
■ Contoh:
  h1 {
    color: red;
    background: blue;
  }
__________________________________________________________________________________
■ CSS selector adalah sebuah penanda, element/tag HTML yang ingin diberi style. Misalnya h1, p, div, dll.
■ Property adalah atribut style yang ingin diubah, misalnya warna teks (color), warna latar belakang (background), ukuran teks (font-size), dsb.
■ Untuk memberikan value pada property CSS, dipisahkan dengan ":" (titik dua) dan diakhiri dengan ";" (titik koma).
■ Value adalah nilai dari property. Misalnya untuk color bisa red, green, blue. Untuk background bisa #fff, #000 dsb.
__________________________________________________________________________________■ Class tidak unik
class bisa digunakan untuk menandai lebih dari satu element, menggunakan simbol .(dot) untuk menandai class.
■ ID bersifat unik
ID hanya boleh digunakan sekali saja untuk satu element. menggunakan simbol #(hash) untuk menandai ID.
__________________________________________________________________________________
■ Untuk melatih kemampuan selector => https://flukeout.github.io/
__________________________________________________________________________________■ Penggunaan comment dalam HTML:
  <!-- ini adalah comment satu baris dalam HTML -->
  <!-- ini adalah comment
  multi baris dalam HTML -->
■ Penggunaan comment dalam CSS:
  /* Ini adalah comment satu baris dalam CSS */
  /* Ini adalah
  comment multi baris
  dalam CSS
  */
__________________________________________________________________________________■ Cara menempatkan CSS:
  ■ Inline CSS: menuliskan CSS langsung pada tag style, contoh:
    <p style="color: blue;">Paragraf biru</p>
  ■ Internal CSS: menuliskan CSS di dalam tag <style> di dalam bagian <head> document HTML, contoh:
    <html>
        <head>
            <style>
            p {
                color: blue;
            }
            </style>
        </head>
    ...
  ■ External CSS: menuliskan CSS di file CSS terpisah dengan ekstensi .css lalu ditautkan ke dalam dokumen HTML menggunakan tag <link> di dalam tag head, contoh:    
    ■ isi file style.css:
      p {
          color: blue;
      }
    ■ Menautkan CSS eksternal ke dalam HTML
      <head>
        <link rel="stylesheet" href="style.css">
      </head>
__________________________________________________________________________________
■ External CSS lebih baik karena:
  ■ Memisahkan konten (HTML) dari tampilan (CSS).
  ■ Mudah dirawat dan diubah, cukup mengubah file CSS saja tanpa menyentuh HTML.
  ■ Lebih efisien dalam hal penggunaan memori dan performa. Browser hanya perlu mengunduh CSS sekali, bukan mengunduh ulang CSS di setiap halaman(Inline CSS dan internal CSS harus diunduh ulang di setiap halaman).
  ■ Mudah berkolaborasi, banyak orang bisa bekerja pada CSS yang sama tanpa perlu menyentuh kode HTML.
__________________________________________________________________________________
■ Beberapa properties CSS yang sering di gunakan:
  ■ background untuk merubah warna latar belakang
  body {
    background: blue;
    color: #ffffff;
  }
__________________________________________________________________________________
  ■ margin adalah sisi luar dari sebuah element, misalnya ingin mengatur jarak antar element. Terdapat beberapa sisi luar margin:
    ■ margin-top yaitu jarak luar atas element
    ■ margin-right yaitu jarak luar kanan element
    ■ margin-bottom yaitu jarak luar bawah element
    ■ margin-left yaitu jarak luar kiri element
  jika menggunakan properties margin saja maka akan otomatis mengatur keempat sisi margin sekaligus. Urutannya atas, kanan, bawah, kiri.
__________________________________________________________________________________  ■ padding adalah sisi dalam sebuah element, misalnya ingin mengatur jarak antara sisi dalam element dengan perbatasannya. Terdapat beberapa sisi dalam padding:
    ■ padding-top yaitu jarak dalam atas element
    ■ padding-right yaitu jarak dalam kanan element
    ■ padding-bottom yaitu jarak dalam bawah element
    ■ padding-left yaitu jarak dalam kiri element
  jika menggunakan properties padding saja maka akan otomatis mengatur keempat sisi padding sekaligus. Urutannya atas, kanan, bawah, kiri.
__________________________________________________________________________________  ■ font untuk mengatur jenis font, ukuran font, style font dll. Beberapa properties untuk mengatur font:
    ■ font-family adalah jenis font, misalnya Arial, Times New Roman, sans-serif
    ■ font-size untuk merubah ukuran font, misalnya 12px, 20pt, larger
    ■ font-weight untk merubah ketebalan font, misalnya normal, bold, bolder, lighter
    ■ font-style untuk merubah gaya font, misalnya normal, italic, oblique
    ■ color untuk merubah warna font, misalnya #fff, #000, blue, green
__________________________________________________________________________________  ■ hyperlink untuk mengatur style link, misalnya warna link, warna link saat dikunjungi, warna link saat di klik. Beberapa properties untuk hyperlink anchor(a):
    ■ a:link untuk merubah status link default
    ■ a:visited untuk merubah status link setelah dikunjungi
    ■ a:active untuk merubah status link saat diklik
    ■ a:hover untuk merubah status link saat diletakkan kursor di atasnya
      ■ contoh:
        a:link {
          color: blue;
          background: white;
        }
__________________________________________________________________________________  ■ format text untuk mengatur format teks, misalnya:
    ■ color
    ■ text-align
    ■ text-decoration
    ■ text-transform
    ■ text-indent
    ■ text-spacing
    ■ word-spacing
    ■ line-height
    ■ text-shadow
    ■ vertical-align
  ■ position untuk mengatur posisi pada sebuah element HTML
    ■ position: relative
    ■ position: absolute
    ■ position: static
    ■ position: fixed
    ■ secara umum untuk membuat posisi atau menetapkan posisi sebuah element kita pasti menggunakan property css lainnya seperti mengatur top, left, bottom, right untuk menetapan posisi sebuah element.
  ■ border untuk mengatur garis border
    ■ border-style: solid
    ■ border-style: dotted
    ■ border-style: dashed
    ■ border-style: double
    ■ border-style: groove
    ■ border-style: inset
    ■ border-style: outset
    ■ border-style: ridge
  ■ list css
    ■ CSS sangat berguna ketika ingin membuat daftar list dengan model tertentu misalnya list yang berbentuk angka, titik, angka romawi dan lainnya.
    ■ Dengan menggunakan CSS kita dapat memanipulasi list HTML dengan mengubah bentuk tanda listnya. untuk mengubah list HTML dengan CSS bisa menggunakan property “list-style-type” yang berarti tipe gaya list.
__________________________________________________________________________________■ Responsive web
  @media(min-width:992px) {
       .selector { 
             width:970px; 
        }
  } 

  @media(max-width:768px) {
        .selector { 
              width:750px;
        }
  }
  ■ Kode yang pertama adalah kode css untuk mendeskripsikan bahwa kode yang ada diantara kurung kurawal pertama & terakhirnya hanya digunakan untuk perangkat yang resolusinya 992 pixel atau lebih (untuk Komputer/Laptop). 

  ■ Kode yang kedua adalah kode css untuk mendeskripsikan bahwa kode yang ada diantara kurung kurawal pertama & terakhirnya hanya digunakan untuk perangkat yang resolusinya 768 piksel atau lebih kecil (untuk Tablet).
__________________________________________________________________________________■ GITHUB
  ■ email student : (blm teregistrasi ke github) 
  ■ di daftarkan github student > membutuhkan KTM > valid until date (ditambahkan)
  ■ https://education.github.com/benefits?type=student
  ■ jika kita sudah pnya github > email student di tambah (secondary email)
■ jika sudah ada github 
  ■ change credentials
  git config --global user.name ""
  git config --global user.email "@gmail.com"
  git config --global credential.username ""

  ■ yang ini untuk kelanjutan nya
  git add .
  git commit -m "update data"
  git push

■ repository : b13a_web_programmer
  b13a_web_programmer :
	  > sesi-01 > beserta file/koding nya
    > sesi-02 > beserta file/koding nya
    > dst


