■ ALGORITMA
  ■ Algoritma adalah serangkaian urutan langkah-langkah yang tepat, logis, terperinci, dan terbatas untuk menyelesaikan suatu masalah yang disusun secara sistematis.
__________________________________________________________________________________
■ Kenapa Algoritma?
  ■ Algoritma adalah inti dari ilmu komputer;
  ■ Algoritma adalah urutan-urutan dari instruksi atau langkah-langkah untuk menyelesaikan suatu masalah;
  ■ Algoritma adalah blueprint dari program;
  ■ Sebaiknya disusun sebelum membuat program.
__________________________________________________________________________________
■ Kriteria Algoritma
  ■ Ada input dan output
  ■ Efektifitas dan efisien
  ■ Terstruktur
__________________________________________________________________________________
■ Contoh Algoritma Bagaimana menggunakan laptop sehari-hari
  ■ Input
    1. Menekan tombol On/Off
    3. Memasukkan Password
    5. Pilih Aplikasi yang mau dibuka
  ■ Output
    2. Menunggu halaman booting
    4. Menunggu validasi password
__________________________________________________________________________________
■ Contoh Algoritma TUKAR ISI EMBER
  ■ Diberikan 2 buah ember A dan B, ember A berisi larutan berwarna merah, ember B berisi larutan berwarna biru. Tukarkan isi kedua ember itu sedemikian sehingga ember A berisi larutan warna biru dan ember B berisi larutan berwarna merah.
    ■ Deskripsi:
      ■ Tuangkan larutan dari ember A ke dalam ember B
      ■ Tuangkan larutan dari ember B ke dalam ember A
      ■ Algoritma TUKAR ISI EMBER di atas tidak menghasilkan pertukaran yang benar.
  ■ Langkah di atas tidak logis, hasil pertukaran yang terjadi adalah pertukaran  kedua larutan tersebut.
  ■ Supaya logis seperti apa?
    ■ Deskripsi:
      ■ Tuangkan larutan dari bejana A ke dalam ember C.
      ■ Tuangkan larutan dari bejana B ke dalam ember A.
      ■ Tuangkan larutan dari bejana C ke dalam ember B.
__________________________________________________________________________________
■ MENGAPA ALGORITMA ITU PENTING?
  ■ Algoritma harus berhenti setelah menjalankan sejumlah langkah terbatas.
  ■ Setiap langkah harus didefinisikan dengan tepat dan tidak berarti-dua (ambiguitas).
  ■ Algortima memiliki nol atau lebih masukan.
  ■ Algoritma memiliki nol atau lebih keluaran.
  ■ Algoritma harus efektif (setiap langkah sederhana sehingga dapat dikerjakan dalam waktu yang masuk akal).
__________________________________________________________________________________
■ Notasi Algoritma:
  1. Penulisan algoritma tidak tergantung dari spesifikasi bahasa pemrograman dan komputer yang mengeksekusinya. Notasi algoritma bukan notasi bahasa pemrograman tetapi dapat diterjemahkan ke dalam berbagai bahasa pemrograman.
  2. Notasi algoritma dapat berupa:
    ■ Uraian kalimat deskriptif (narasi)
__________________________________________________________________________________
■ Algoritma kelulusan mahasiswa
  ■ Diberikan nama dan nilai mahasiswa, jika nilai tersebut lebih besar atau sama dengan 60 maka mahasiswa tersenut dinyatakan lulus, jika nilai lebih kecil dari  60 maka dinyatakan tidak lulus.
  ■ Baca nama dan nilai mahasiswa  Jika nilai >= 60 maka  Keterangan = lulus
  ■ Tetapi jika salah  Keterangan = tidak lulus  Tulis nama dan keterangan.
__________________________________________________________________________________
■ LATIHAN BERPIKIR ALGORITMA
  ■ Flowchart
    ■ Flowchart adalah bagan-bagan yang mempunyai arus menggambarkan langkah-langkah penyelesaian suatu masalah
    ■ Merupakan cara penyajian dari suatu algoritma
    ■ Ada 2 macam flowchart:
      ■ System flowchart:
        ■ Urutan proses dalam system dengan menunjukkan alat media input, output serta jenis penyimpanan  dalam proses pengolahan data.
      ■ Program flowchart:
        ■ Urutan instruksi yang digambarkan dengan symbol tertentu untuk memecahkan masalah dalam suatu  program.
__________________________________________________________________________________
  ■ Contoh nama beberapa simbol Flowchart
    ■ Flow Direction Symbols (simbol penghubung alur)
    ■ Processing Symbols (simbol proses)
    ■ Input-Output Symbols (simbol input-output)
__________________________________________________________________________________
■ PSEUDOCODE
■ Dalam menggunakan bahasa pemrograman, kita bisa menggunakan atau bahkan tidak perlu menggunakan algoritma. Tapi hampir 99% pastinya perlu algoritma. Misalnya saja kita sudah tahu algoritma dasar dari perulangan dan perkondisian. Mengenal Pseudocode Atau agar lebih rapi, kita gunakan pseudocode.
■ Psedudocode adalah konvensi terstruktur atau cara menyajikan penjelasan algoritma dengan bahasa yang deskriptif seperti kita menulis kalimat biasa sehingga mudah kita baca. Umumnya digunakan bahasa Inggris atau bahasa perantara yang mirip bahasa pemrograman.
__________________________________________________________________________________
■ Contoh algoritma penambahan angka sederhana dengan pseudocode
■ Contoh dengan Bahasa Inggris
  ■ READ and SAVE "first number"
  ■ READ and SAVE "second number"
  ■ COMPUTE "first number" added by "second number"
  ■ SAVE previous computation result
  ■ SHOW the computation result
__________________________________________________________________________________
■ Bahasa inggris diatas nantinya akan diubah menjadi bahasa pemrograman yang kita mau.
■ Contoh hasil konversi pseudocode diatas menjadi kode di bahasa lain.
  ■ Bahasa pemrograman python
    a = input("First Number? ")
    b = input("Second Number? ")
    c = int(a) + int(b)
    print(f"Result {c}")
  ■ Bahasa pemrograman Ruby
    puts "First Number?"
    a = gets.chomp
    puts "Second Number?"
    b = gets.chomp
    c = a.to_1 + b.to_1
    puts c
  ■ Bahasa pemrograman Javascript
    var a, b, c;
    a = prompt("First Number?");
    b = prompt("Second Number?");
    c = Number(a) + Number(b);
    console.log(c);
    alert("Result = " + c);
__________________________________________________________________________________
■ Pseudocode tidak terpaku pada penggunakan kata tertentu. Selama pseudocode dapat dimengerti sesama pembaca, maka sudah cukup bisa digunakan. Kita bisa menggunakan huruf kapital untuk keyword yang ditekankan dari sebuah step.
  ■ Misal: CALCULATE 5 plus 2, atau DISPLAY "hello".
__________________________________________________________________________________
■ Storing Values
  ■ Biasanya, pada saat kita belajar matematika atau fisika, kita akan bertemu dengan rumus. Paling sederhana adalah rumus luas persegi, yaitu width dikalikan height.
  ■ Kita sebagai manusia dengan natural dapat langsung mengkalkulasi nilai panjang dan lebar untuk mendapatkan luas. Tapi, komputer tidak semudah itu. Komputer harus menyimpan nilai panjang dan nilai lebar di dalam memori. Memori komputer, bayangkan saja seperti otak kita yang bisa menyimpan berbagai informasi. Sebetulnya, saat kita menghitung panjang dan lebar secara tidak sadar kita pun menampung nilai tersebut di kepala kita.
__________________________________________________________________________________
  ■ Contoh pseudocode:
    STORE "width" with any value
    STORE "height" with any value
    STORE "area" without any value

    Calculate "width" times "height"
    SET "area" value with calculatin result
    DISPLAY "area"
__________________________________________________________________________________
  ■ Bisa dilihat dari pseudocode diatas, ada beberapa step yang kita jalankan. Mari kita bahas tiap step ke bahasa yang lebih "manusiawi"
    ■ Simpan "width" dengan nilai berapapun
    ■ Simpan "height" dengan nilai berapapun
    ■ Simpan "area" tanpa diberikan nilai. Ini akan kita isi nanti.

    ■ Hitung hasil perkalian "width" dengan "height"
    ■ Setelah mendapatkan hasil perhitungan, isikan hasilnya ke dalam "area"
    ■ Tampilkan nilai dari "area"
__________________________________________________________________________________
■ Conditional
  ■ Saat komputer menjalankan program, seringkali komputer harus melakukan sebuah tindakan jika suatu kondisi terpenuhi. Mudahnya, di kehidupan sehari-hari misalnya, jika kita lapar, kita akan makan. "Jika kita lapar" adalah sebuah kondisi, dan "kita akan makan" adalah step yang hanya akan dijalankan apabila kondisi tersebut terpenuhi.
  ■ Contoh dalam pseudocode:
    IF "hungry"
      DO "eat"
    DISPLAY "i am happy"
  ■ Jika kita lihat pseudocode diatas, bisa dijabarkan sebagai step berikut
  ■ Jika lapar, maka masuk ke step 2. Jika tidak, abaikan step 2 dan langsung ke step 3. lakukan proses "eat" Tampilkan "i am happy" Yang terjadi disini ada dua kemungkinan. Jika lapar, step 2 akan diabaikan. Kita bisa lihat dari pseudocode dimana "eat" kita buat menjorok ke dalam (ingat dengan identasi di HTML? ya betul!) untuk menunjukkan semua proses yang menjorok ke dalam setelah sebuah kondisi merupakan proses yang dijalankan hanya jika kondisi terpenuhi.
  ■ Tidak hanya sampai disana, kondisional bisa juga melakukan proses yang hanya dijalankan jika kondisi tidak terpenuhi. Misal, saat nilai ujian dibawah 70, saya harus berlajar lebih giat. Tapi jika tidak, maka saya layak memberi reward untuk diri sendiri.
  ■ Contoh dalam pseudocode:
    STORE "score" to any number
__________________________________________________________________________________
    IF "score" < 70
      DO "learn more"
    ELSE
      DO "reward myself"
    DO "continue with life..."
  ■ Nah disini terjadi yang biasa dinamakan percabangan. Jika score dibawah 70, maka kita akan "learn more", dan jika tidak, maka kita harus "reward myself". Namun apapun kondisinya, kita pasti akan masuk ke step "continue with life..."
  ■ Pseudocode diatas bisa digambarkan ke step berikut:
    ■ Jika "score" dibawah 70, masuk ke step 2a. Jika tidak, masuk ke step 2b. 2a. Lakukan "learn more" 2b. Lakukan "reward myself" Lakukan "continue with life..."
    ■ Saat program berjalan, berarti hanya ada dua kemungkinan. Antara menjalankan step 1 -> 2a -> 3, atau step 1 -> 2b -> 3.
__________________________________________________________________________________
■ Looping(perulangan)
  ■ Komputer seringkali dibutuhkan untuk melakukan sebuah proses yang sama berulang-ulang. Hal ini sering disebut sebagai looping. Tentunya, saat komputer melakukan looping, pasti ada kalanya proses tersebut akan berhenti. Sama hal nya saat kita sebagai manusia melakukan berbagai hal yang berulang, pasti ada kalanya kegiatan itu kita hentikan. Nah, looping sebetulnya melibatkan yang sudah kita pelajari sebelumnya, yaitu conditional. Looping akan terus dilakukan sampai sebuah kondisi terpenuhi. Contoh mudahnya adalah, kita akan makan hingga kenyang bukan?
__________________________________________________________________________________
  ■ Contoh pseudocode:
    WHILE "hungry"
      DO "eat"
__________________________________________________________________________________
    ■ Nah, pseudocode di atas cukup simple dan mencontohkan kita proses paling sederhana dalam looping. WHILE adalah standard keyword untuk menunjukkan kondisi "selama kita masih lapar", lakukan proses makan.
    ■ Biasanya, saat kita membuat looping, ada sebuah proses yang dilakukan untuk mencapai kondisi tersebut. Kita coba perbaiki contoh pseudocode diatas, dengan asumsi kemampuan makan kita dalam sekali makan adalah 5 sendok nasi. Kita coba umpakan kemampuan makan ini sebagai "hungry level".
__________________________________________________________________________________
    STORE "full level" with 0

    WHILE "full level" < 5
      ADD "full level" by 1

    DISPLAY "I'm full!"
__________________________________________________________________________________
    ■ Nah, looping kali ini sudah lebih mendekati coding sebenarnya. Saat terjadi looping, harus ada proses apapun yang akan membuat kondisi perulangan lambat laun akan terpenuhi. Pseudocode di atas menggambarkan kita mulai dari level kenyang kita dari 0, berarti kita saat ini sangat lapar. Setiap kali kita melakukan proses makan, tingkat kenyang kita akan bertambah 1. Karena kita hanya kuat makan hingga 5 kali, maka kondisinya adalah "full level" < 5.
__________________________________________________________________________________
    ■ Kita coba ilustrasikan step pseudocode diatas:
      ■ Simpan nilai "full level" dengan angka 0
      ■ Ulangi step 3 selama "full level" masih dibawah 5. Jika "full level" sudah 5, lanjut ke step 4.
      ■ Tambah "full level" dengan 1, agar semakin mendekati batas perulangan. Kembali ke step 2.
      ■ Tampilkan "I'm full", berarti saya sudah sangat kenyang!
__________________________________________________________________________________
    ■ Contoh lain membuat pesudocode yang menggunakan looping dan conditional sekaligus
    ■ Seorang anak SD sedang belajar angka genap dan ganjil. Dia ditugaskan oleh ibu guru untuk menghitung angka dari 1 sampai 10 dengan menyebut angka tersebut dan untuk setiap angka ganjil, ia harus menyebut "ODD" dan sebaliknya jika genap, ia harus menyebut "EVEN"
      ■ Dalam pseudocode sisa bagi di sebut MOD/MODULUS artinya untuk mencari nilai genap maka kita bisa menggunakan MOD 2 == 0, untuk mencari angka ganjil artinya sebaliknya karena ganji tidak habis di bagi 2.
__________________________________________________________________________________
      ■ Psoudocodenya:
        STORE "count" AS 1

        WHILE "count" < 11
          DISPLAY "count"
          COMPUTE "count" mod 2
          STORE "reminder" to result of calculation

          IF "reminder" EQUALS 0
            DISPLAY "EVEN"
          ELSE
            DISPLAY "ODD"

          COMPUTE "count" + 1
          STORE "count" to result of calculation