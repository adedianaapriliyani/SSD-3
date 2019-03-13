
<h1> SIMULASI MENEJEMEN PROYEK PERANGKAT LUNAK (SSD)</h1>
<b>1. Pendahuluan</b><br>
&emsp;<b>1.1 Tujuan</b><br>
&emsp;&emsp;Untuk pengembangan versi pertambahan software secara cepat. untuk menyelesaikan sistem secara global terlebih dahulu, kemudian untuk feature dari sistem akan dikembangkan kemudian. Sehingga mempercepat dalam pengimplementasian project. <br>
&emsp;<b>1.2 Lingkup</b><br>
&emsp;&emsp;Ruang lingkup dokumen SSD ini adalah penjelasan mengenai desain aplikasi Sistem Menejemen Proyek secara rinci. Ruang lingkup sistem ini mencakup informasi mengenai antar muka dari sistem tersebut. Sistem 
ini memungkinkan user untuk melakukan order proyek, dengan cara input data melalui aplikasi mangoline tersebut, nantinya sistem ini akan menghitung berapa cost yang harus dikeluarkan untuk menunjang sistem tersebut. Sistem ini juga memungkinkan untuk melakukan penyimpanan history dari kegiatan konsumen, melakukan penambahan produk, dan histori laporan.<br>
&emsp;<b>1.3 Definisi, Akronim, Singkatan</b><br>
&emsp;&emsp;Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website (MANGOLINESHP) adalah salah satu jenis aplikasi 
&emsp;&emsp;perangkat lunak yang dapat digunakan untuk membantu proses penjualan olahan secara online. Selama ini pemasaran 
&emsp;&emsp;olahan mangga khas Indramayu dipasarkan secara konvensional yaitu dijual di toko sekitar Indramayu saja.<br>
&emsp;<b>2 Referensi</b><br>
&emsp;&emsp;a.	Modul KULIAH RPL 7 DOKUMEN SDD <br>
&emsp;&emsp;b.	Contoh Software Design Document (SDD) Moch. Bambang Sulistio <br>
&emsp;<b>3 Penjelasan Dekomposisi </b><br>
&emsp;&emsp;<b>3.1 Dekomposisi Modul</b><br>
&emsp;&emsp;&emsp;<b>3.1.1 Deskripsi Modul 1</b><br>
&emsp;&emsp;&emsp;&emsp;Kebutuhan fungsional (Functional Requirements) ini adalah kebutuhan utama yang diharapkan dari sistem ini, yang &emsp;&emsp;&emsp;&emsp; terkait langsung dengan sistem ini. <br>
&emsp;&emsp;&emsp;&emsp;Kebutuhan fungsional dari sistem ini adalah sebagai berikut:<br>
&emsp;&emsp;&emsp;&emsp;1.	Pencatatan Hak Akses <br>
&emsp;&emsp;&emsp;&emsp;2.	Pencatatan Nama aplikasi , Nama Kategori dan Nama Client <br>
&emsp;&emsp;&emsp;&emsp;3. Pencatatan Target Waktu , Jumlah Orang dan Biaya Aplikasi <br>
&emsp;&emsp;&emsp;&emsp;Spesifikasi yang diharapkan pada Pencatatan Hak Akses: <br>
&emsp;&emsp;&emsp;&emsp;•	Membedakan antara user dan admin dalam hak ases <br>
&emsp;&emsp;&emsp;&emsp;•	Sistem dapat memproses secara otomatis jika kita terdaftar dalam admin memiliki hak ases penuh dan sebaliknya &emsp;&emsp;&emsp;&emsp;juka terdaftar dalam user tidak memiliki hak ases penuh 
Spesifikasi yang diharapkan pada Pencatatan Nama aplikasi,&emsp;&emsp;&emsp;&emsp;Nama Kategori <br>
&emsp;&emsp;&emsp;<b>3.1.2 Deskripsi Modul 2</b><br>

&emsp;&emsp;&emsp;&emsp;Nama  Client : <br>
&emsp;&emsp;&emsp;&emsp;•	Mencatat nama aplikasi apa yang akna di buat dalam sebuah project <br>
&emsp;&emsp;&emsp;&emsp;•	Mencatat nama-nama kategori apa yang akan di buat di sebuah project <br>
&emsp;&emsp;&emsp;&emsp;•	Mencatat nama client yang mau di buat kan sebuah project <br>
&emsp;&emsp;&emsp;&emsp;Spesifikasi yang diharapkan pada Pencatatan Target Waktu , Jumlah Orang dan Biaya Aplikasi : <br>
&emsp;&emsp;&emsp;&emsp;•	Sistem dapat memproses secara otomatis target waktu aplikasi yang akan di buat dalam sebuah project  <br>
&emsp;&emsp;&emsp;&emsp;•	Sistem dapat memproses secara otomatis jumlah orang dalam sebuah project  <br>
&emsp;&emsp;&emsp;&emsp;•	Sistem dapat memproses secara otomatis biaya dalam sebuah aplikasi yang akan di buat <br>

&emsp;&emsp;<b>3.2 Dekomposisi Proses Konkuren</b><br>
&emsp;&emsp;&emsp;<b>3.2.1 Deskripsi Proses 1</b><br>
&emsp;&emsp;&emsp;&emsp;Konkurensi adalah proses-proses (lebih dari satu proses) yang terjadi pada saat bersamaan. Konkurensi merupakan &emsp;&emsp;&emsp;&emsp; landasan umum perancangan sistem operasi. <br>
&emsp;&emsp;&emsp;&emsp;Proses-proses disebut konkuren jika proses-proses berada pada saat yang sama. Pada proses-proses konkuren yang &emsp;&emsp;&emsp;&emsp; berinteraksi mempunyai beberapa masalah yang harus diselesaikan: <br>
&emsp;&emsp;&emsp;&emsp;1.	Mutual Exclusion <br>
&emsp;&emsp;&emsp;&emsp;2.	Sinkronisasi <br>
&emsp;&emsp;&emsp;&emsp;3.	Deadlock <br>
&emsp;&emsp;&emsp;&emsp;4.	Startvation <br>

&emsp;&emsp;&emsp;<b>3.2.2 Deskripsi Proses 2</b><br>
&emsp;&emsp;&emsp;&emsp;Pada sistem dengan banyak proses (kongkuren), terdapat 2 katagori interaksi, yaitu: <br>
&emsp;&emsp;&emsp;&emsp;1.	Proses-proses Saling Tidak Peduli (Independen). <br>
&emsp;&emsp;&emsp;&emsp;Proses-proses ini tidak dimaksudkan untuk bekerja untukmencapai tujuan tertentu. Pada multiprogramming dengan  &emsp;&emsp;&emsp;&emsp;proses-proses independen, dapat berupa batch atau sesi interaktif, atau campuran keduanya. <br>
&emsp;&emsp;&emsp;&emsp;2.	Proses-proses Saling Mempedulikan Secara Tidak Langsung. <br>
&emsp;&emsp;&emsp;&emsp;Proses-proses tidak perlu saling mempedulikan identitas proses-proses lain, tapi sama-sama mengakses&emsp;&emsp;&emsp;&emsp;objek tertentu, seperti buffer masukan/keluaran. Proses-proses itu perlu bekerja sama (cooperation) dalam memakai bersama objek&emsp;&emsp;&emsp;&emsp;tertentu.  <br>
&emsp;&emsp;&emsp;&emsp;3.	Proses-proses konkuren mengharuskan beberapa hal yang harus ditangani, antara lain: <br>
&emsp;&emsp;&emsp;&emsp;a.	Sistem operasi harus mengetahui proses-proses yang aktif <br>
&emsp;&emsp;&emsp;&emsp;b.	Sistem operasi harus mengalokasikan dan mendealokasikan beragam sumber daya untuk tiap proses aktif. &emsp;&emsp;&emsp;&emsp; Sumber daya yang harus dikelola, antara lain: <br>
&emsp;&emsp;&emsp;&emsp;1.	Waktu pemroses. <br>
&emsp;&emsp;&emsp;&emsp;2.	Memori <br>
&emsp;&emsp;&emsp;&emsp;3.	Berkas-berkas <br>
&emsp;&emsp;&emsp;&emsp;4.	Perangkat I/O <br>
&emsp;&emsp;&emsp;&emsp;c.	Sistem operasi harus memproteksi data dan sumber daya fisik masingmasing proses dari gangguan proses-proses &emsp;&emsp;&emsp;&emsp; lain. <br>
&emsp;&emsp;&emsp;&emsp;d.	Hasil-hasil proses harus independen terhadap kecepatan relatif prosesproses lain dimana eksekusi dilakukan. <br>

&emsp;&emsp;<b>3.3 Dekomposisi Data</b><br>
&emsp;&emsp;&emsp;<b>3.3.1 Deskripsi Entri data 1</b><br>
&emsp;&emsp;&emsp;&emsp;Bagian ini akan menjelaskan struktur data. Table yang terbentuk ada 2 (Dua) dengan nama masing masing tablenya &emsp;&emsp;&emsp;&emsp; adalah sebagai berikut : <br>
&emsp;&emsp;&emsp;&emsp;•	Tabel karyawan <br>
&emsp;&emsp;&emsp;&emsp;•	Tabel hitung_cost <br>

&emsp;&emsp;&emsp;<b>3.3.2 Deskripsi Entri data 2</b><br>
&emsp;&emsp;&emsp;Tabel hitung, digunakan untuk menyimpan hasil efroth, durasi waktu, jumlah orang dan gaji setiap karyawan yang &emsp;&emsp;&emsp;&emsp; bekerja dalam sebuah project aplikasi. <br>
<b>4. Deskripsi Ketergantungan/Keterkaitan</b><br>
&emsp;&emsp;<b>4.1 Keterkatian inter modul</b><br>
&emsp;&emsp;Ketika merancang sebuah Dependensi Inter-modul sistem, dapat dirancang dengan dua cara yang luas dan cara pertama adalah untuk merancang sistem yang lengkap dengan menggunakan sistem yang ada diketahui dan mengimplementasikan fitur baru yang diperlukan untuk meningkatkan efektivitas sistem dan mengujinya di kondisi nyata. Cara alternatif akan merancang sistem dan biasanya karena biaya untuk menyiapkan antarmuka antara modul. Modul dari siaran berita Sistem SSD tergantung pada penyebaran informasi. Ini antar-modul dari penelitian ini adalah tampilan dari pengumuman dan itu termasuk database sistem. Kemudian seluruh informasi yang telah dimasukkan akan disimpan dalam database, yang berasal dari proses input sampai pengumuman menampilkan ke monitor lain.<br>
&emsp;&emsp;<b>4.2 Keterkatian inter modul</b><br>
&emsp;&emsp;Proses yang dilakukan oleh pengguna dalam melakukan pemesanan proyek aplikasi akan mempengaruhi beberapa proses lainya seperti penentuan value, dan penjadwalan. Juga data akan tersimpan sebagai riwayat proses pemesanan<br>
&emsp;&emsp;<b>4.3 Keterkaitan data</b><br>
&emsp;&emsp;Dependensi data didasarkan pada pengguna. Mereka adalah orang yang akan memverifikasi atau menyetujui pengumuman antri<br>
<b>III.5 DESKRIPSI ANTARMUKA</b><br>
&emsp;&emsp;<b>III.5.1 Deskripsi Antarmuka Pengguna</b><br>
&emsp;&emsp;Antarmuka pengguna (user interface) merupakan bentuk tampilan grafis yang berhubungan langsung dengan pengguna (user). Antarmuka pengguna berfungsi untuk menghubungkan antar pengguna dengan sistem, sehingga sistem tersebut bisa digunakan. Berikut merupakan rangcangan desain antarmuka pengguna proyek kami.<br>
<img src="/img/1.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Gambar Form awal]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk melakukan proses login guna mendapatkan hak akses ke aplikasi. Untuk mendapat akses masuk ke dalam sistem, user harus menginputkan user name dan password dengan benar pada textbox yang telah disediakan . kemudian sistem akan mengecek user name dan password yang dimasukkan dengan data user name dan password yang telah tersimpan di dalam sistem. Jika data user name dan password cocok maka pengguna akan diberikan akses masuk ke dalam sistem, sebaliknya jika user name dan password salah atau tidak cocok maka akan ada pesan peringatan dari aplikasi.<br>
<img src="/img/2.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Gambar Form menu]</b><br>
&emsp;&emsp;Antarmuka ini merupakan antarmuka utama yang berisi menu untuk masuk ke antarmuka-antarmuka yang lain. User dapat meilih fungsionalitas- fungsionalitas yang ditawarkan oleh aplikasi. Fungsionalitas yang ditawarkan seperti pembuatan proyek, info karyawan, dan perhitungan cost.<br>
<img src="/img/3.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[form pesan produk]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk membuat proyek perhitungan yang di inginkan. Untuk membuat proyek user harus mengisi form yang telah disediakan, kemudian meng-click hitung. Dan kemudian user diharuskan meng-click save yang berada di pojok kanan atas. Secara otomatis proyek akan disimpan.<br>
<img src="/img/4.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Form data karyawan]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk melihat data para Karyawan, caranya adalah tinggal memasukkan ID Karyawan yang ingin dilihat. Kemudian secara otomatis data akan keluar.<br>
<img src="/img/5.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Form Data pesanan Produk]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk melihat data dari keseluruhan transaksi pesanan proyek yang pernah ada.
<img src="/img/6.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Form data Laporan]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk melihat dokumen-dokumen yang ditunjukan dalam pembangunan Simulasi Manajemen Proyek RPL.<br>
<img src="/img/7.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[Form data dokumen]</b><br>
&emsp;&emsp;Antarmuka ini digunakan untuk melihat data atau informasi dari anggota kelompok tim 2 proyek RPL.<br>
<img src="/img/8.png"><br>
&emsp;&emsp;&emsp;&emsp;<b>[form info kami]</b><br>