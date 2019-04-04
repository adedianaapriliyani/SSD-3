<p align="center"><font size="5"><b>SOFTWARE DESIGN DOCUMENT</b></font><br>
	<font size="5"><b>APLIKASI PENJUALAN OLAHAN</b></font><br>
	<font size="5"><b>BUAH MANGGA INDRAMAYU BERBASIS WEBSITE</b></font><br></p>

<p align="center"><img src="images/polindra.png" width="250" height="250"></p>

<br>

<p align="center">
    <b><font size="4">Kelompok 3:</font></b><br>
    Ade Diana Apriliyani	 (1703072) <br>
    Fany Fahrurozi (1703060)<br>
    Fiqi Andri Reviansyah (1703064)<br>
</p>
<center><font size="3"><p align="center">Kelas D3TI2C</p></font></center>
<br>

<p align="center"><b><font size="5">D3 TEKNIK INFORMATIKA</font></b><br>
<b><font size="3">POLITEKNIK NEGERI INDRAMAYU</font></b><br>
<b><font size="3">2019</font></b></p>
<p>&nbsp;</p>

<p><strong>&nbsp;</strong></p>
<p align="center"><font size="5">Jl. Lohbener Lama No.08, Lohbener, Indramayu, Legok, Lohbener, Kabupaten Indramayu, Jawa Barat 45252, Indonesia</font><br>

<p><strong>&nbsp;</strong></p>


<p align="center"><b><font size="5">KATA PENGANTAR</font></b><br>

<p>&nbsp;</p>
<p>Puji syukur kehadirat Allah swt yang telah melimpahkan rahmat-Nya sehingga aplikasi ini dapat diselesaikan tepat pada waktunya dengan judul &ldquo;Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website &rdquo;. Aplikasi ini disusun demi memenuhi Tugas Mata Kuliah Proyek II Program Studi Teknik Informatika Diploma III Politeknik Negeri Indramayu.</p>
<p>Harapan kami, aplikasi ini menjadi salah satu media yang menarik untuk dikunjungi dan mudah dipahami oleh seluruh pengunjungnya. Akhirnya penyusun mengucapkan banyak terima kasih, khususnya kepada:</p>
<ol>
<li>Ibu Munengsih Sari Bunga, S.Kom., M.Eng selaku Ketua Jurusan Teknik Informatika Politeknik Negeri Indramayu.</li>
<li>Bapak Adi Suheryadi S.ST., M.Kom., selaku dosen wali kelas D3TI.2C dan dosen pembimbing I.</li>
<li>Bapak Eka Ismantohadi, S.Kom.,M.Eng selaku dosen pembimbing II.</li>
<li>Bapak Kurnia Adi Cahyanto, S.T.,M.Kom selaku dosen pembimbing III.</li>
<li>Orang tua dan keluarga yang selalu memberikan dukungan kepada saya baik itu moril maupun materil.</li>
<li>Rekan-rekan D3TI.2C, yang selalu memberikan keceriaan disetiap harinya sehingga saya tidak merasa terbebani dengan adanya tugas ini.</li>
</ol>
<p>Penyusun mengharapkan saran-saran dari para pembaca sebagai masukan yang berguna bagi penyempurnaan aplikasi ini. Semoga aplikasi ini bermanfaat bagi kita semua.</p>
<p><br /> <br /> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Indramayu, 10 Februari 2019<br /> <br /> <br /> <br /> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Penulis</p>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>


<p align="center"><b><font size="5">RINGKASAN</font></b><br>


<p>Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website (MANGOLINESHP) adalah salah satu jenis aplikasi perangkat lunak yang dapat digunakan untuk membantu proses penjualan olahan secara online. Selama ini pemasaran olahan mangga khas Indramayu dipasarkan secara konvensional yaitu dijual di toko sekitar Indramayu saja. Pemasaran olahan mangga Indramayu pun kurang berkembang karena pembeli harus datang ke toko. Oleh karena itu olahan mangga&nbsp; khas Indramayu pun yang mengenal hanya orang-orang yang singgah atau berwisata ke Indramayu saja. Sehingga kami berinisiatif untuk membuat sebuah wadah yang didalamnya terdapat lapak-lapak penjual olahan mangga dalam bentuk aplikasi berbasis website. Dibuatnya aplikasi ini kami bisa membantu pemasaran dari penjual olahan mangga Indramayu serta mempromosikan tentang keberagaman olahan mangga yang ada di Indramayu.</p>
<p>Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website ini dibangun dengan menggunakan framework laravel dengan didukung basis data MYSQL.</p>
<p><strong>Kata kunci&nbsp;&nbsp;&nbsp;&nbsp; : </strong>Aplikasi Penjualan, framework laravel, MYSQL</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong><br /> </strong></p>
<p><strong>&nbsp;</strong></p>

<p align="center"><b><font size="5">BAB I</font></b><br>
<b><font size="3">PENDAHULUAN</font></b></p>

<li><strong>1.1	Tujuan</strong></li>

<p>Tujuan pembuatan SDD (Software Design Description) ini   adalah untuk menjelaskan langkah langkah desain dan proses-proses dalam pembuatan sistem aplikasi yang akan diterapkan pada Aplikasi Mangolineshop (Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website), dan juga memberi definisi kebutuhan untuk sistem, spesifikasi kebutuhan fungsional. 
Fungsi utama dari aplikasi Mangolineshop ini adalah mempermudah penjual olahan mangga dalam memberikan pelayanan terhadap pembeli, memudahkan penjual dalam rekap laporan keuangan, dan sebagai sarana untuk mempromosikan produk olahan mangga khas Kota Indramayu.
Secara ringkas, fungsi Aplikasi Mangolineshop dapat dituliskan sebagai berikut : 
</p>
<ol>
<li>Admin dapat menginputkan fitur kategori produk, akun penjual, dan akun pembeli yang nantinya akan digunakan oleh user dalam aplikasi tersebut.</li>
<li>Admin merekap laporan transaksi.</li>
<li>Aplikasi penjual harus mendaftar terlebih dahulu di admin Mangolineshop.</li>
<li>Aplikasi penjual dan admin login, kemudian memberikan detail produk olahan mangga pada pembeli.</li>
<li>Pembeli harus melakukan konfirmasi pembelian terlebih dahulu setelah memilih produk olahan mangga yang ingin dibeli pada aplikasi Manolineshop.</li>
<li>Pembeli melakukan pembayaran setelah konfirmasi pemesanan menu – menu yang dibeli di aplikasi kasir sebagai bukti pembayaran</li>
<li>Aplikasi penjual dan admin login, kemudian melakukan proses perhitungan pembayaran untuk pembeli.</li>
<li>8.	Setelah melakukan transaksi penjual dan admin dapat melihat laporan pendapatan terhadap pemesanan yang dilakukan oleh pembeli. </li>
</ol>
<p>&nbsp;</p>

<li><strong>1.2	Ruang Lingkup</strong></li>

<p>Hasil dari SDD ini adalah aplikasi yang berbasis web, yang digunakan untuk membantu pemasaran dan pengelolaan yang ada di UKM Kenanga Mandiri dalam hal :</p>
<ol>
	<li>Mencatat produk olahan mangga Indramayu yang akan ditampilkan di aplikasi Mangolineshop.</li>
	<li>Mencatat pemesanan produk olahan mangga terhadap pembeli di aplikasi Mangolineshop.</li>
	<li>Menghitung transaksi terhadap pemesanan yang dilakukan oleh pembeli yang akan dilakukan pada aplikasi Admin dari aplikasi Mangolineshop.</li>
	<li>Mencatat laporan transaksi yang akan ditampilkan di aplikasi penjual dan admin dari aplikasi Mangolineshop.</li>
</ol>



<li><strong>1.3	Gambaran umum dokumen</strong></li>

<p>Penulisan dokumen ini dibagi menjadi beberapa bab sebagai berikut: </p>
<ol>
	<li>Bab 1, adalah Pendahuluan yang menjelaskan mengenai tujuan perangkat lunak, ruang lingkup, serta gambaran umum dokumen. </li>
	<li>Mencatat pemesanan produk olahan mangga terhadap pembeli di aplikasi Mangolineshop.</li>
	<li>Bab 2, adalah Deskripsi Umum, yang berisi tentang gambaran umum mengenai perspektif produk, manfaat produk, karakteristik user dan stakeholder, batasan, serta asumsi dan ketergantungan yang digunakan. </li>
	<li>Bab 3, adalah Software Design, yang menyediakan spesifikasi, kebutuhan, antarmuka, kebutuhan fungsional dan nonfunctional, lingkungan operasi, dan batasan perancangan, permodelan proses, permodelan data, struktur data, spesifikasi program dan desain interface.</li>
	</ol>
	
<p align="center"><b><font size="5">BAB III</font></b><br>
<b><font size="3">SOFTWARE DESIGN</font></b></p>

<li><strong>3.1	Kebutuhan Fungsional</strong></li>
<p>Kebutuhan fungsional (Functional Requirements) ini adalah kebutuhan utama yang diharapkan dari sistem ini, yang terkait langsung dengan sistem ini. Kebutuhan fungsional dari sistem ini adalah sebagai berikut:</p>
<ol>
<li>1.	Pencatatan pesanan</li>
<li>2.	Pencatatan laporan keuangan</li>
<li>3.	Manajemen produk olahan mangga Indramayu</li>
<li>4.	Transaksi</li>
</ol>
<p>Spesifikasi dari system yang diharapkan:</p>
<p>1.	Spesifikasi yang diharapkan pada Pencatatan Pesanan</p>
<ol>
<li>a.	Sistem dapat mencatat pesanan yang telah dipilih melalui website.</li>
<li>b.	Sistem dapat mengcancel pesanan yang sudah dipilih sebelum konfirmasi pesanan.</li>
<li>c.	Sistem dapat memberikan pemberitahuan jika barang sudah tidak tersedia maka pembeli atau reseller tidak dapat melakukan pemesanan produk.</li>
</ol>
<p>2.	Spesifikasi yang diharapkan dari laporan keuangan</p>
<ol>
<li>a.	Sistem dapat menampilkan pendapatan hari ini</li>
<li>b.	Sistem dapat menampilkan laporan keuangan dalam periode waktu tertentu</li>
</ol>
<p>3.	Spesifikasi yang diharapkan pada Manajemen produk olahan mangga Indramayu</p>
<ol>
<li>a.	Sistem harus dapat menghapus, dan menambah produk olahan mangga Indramayu </li>
<li>b.	Sistem dapat menampilkan produk olahan mangga Indramayu yang masih tersedia<lli>
</ol>
<p>4.	Transaksi</p>
<ol>
<li>a.	Sistem harus dapat menghitung harga yang harus dibayar pembeli. Dan jika ada yang mau menjadi reseller maka system dapat membedakan harga yang harus dibayar reseller.</li>
<li>b.	Sistem harus dapat menghitung data pesanan</li>
</ol>
<li><strong>3.2	Kebutuhan Non Fungsional</strong></li>
<p>Kebutuhan yang mendukung kelancaran sistem ini didefnisikan sebagai berikut:</p>
<ol>
<li>Availability	:</li>
<p>Aplikasi secara online, dengan asumsi koneksi internet dan jaringan berjalan normal</p>
<li>Reliability	: </li>
<p>Sistem data reliabel berhubungan dengan stok produk olahan mangga Indramayu dan juga reliabel berhubungan dengan laporan keuangan</p>
<li>Ergonomy	:</li>
<p>User friendly dengan memperhatikan hal yang berhubungan dengan Human Computer Interaction</p>
<li>Portability	: </li>
<p>Dapat diakses dari website untuk produk olahan mangga Indramayu serta diakses dari desktop mengenai transaksi dan laporan</p>
<li>Memory 	: </li>
<p>Minimum memory untuk server aplikasi 4 Gb</p>
<li>Response time: </li>
<p>Tidak terukur</p>
<li>Security	:</li>
<p>Login dan validasi password</p>
</ol>
<li><strong>3.3	Kebutuhan Antarmuka (interface)</strong></li>
<p>Antarmuka dalam penerapan aplikasi Mangolineshop dibagi menjadi dua, yaitu:</p>

<p>1.	Hardware Interface	: adalah kebutuhan perangkat keras yang harus dipenuhi untuk implementasi sistem aplikasi Mangolineshop berbasis website.</p>
<p>2.	Software Interface	: kebutuhan software untuk implementasi sistem aplikasi Mangolineshop:</p>
<ol>
<li>Postgre </li>
<li>Server Laragon</li>
<li>Visual Studio Code</li>
<li>Google Crome</li>
<li>Mozilla Firefox</li>
</ol>
	
<li><strong>3.4	Lingkungan Operasi</strong></li>
<p>Aplikasi aka berfungsi dengan lingkungan operasi sebagai berikut:</p>
<ol>
<li>Sistem Operasi 	: Windows </li>
<li>DBMS		: Berbasis Postgre</li> 
<li>Pemrograman		: PHP dan HTML</li>
</ol>

<li><strong>3.5	Batasan Perancangan</strong></li>
<p>Perancangan sistem aplikasi Mangolineshop ini adalah berbasis website untuk admin, penjual, reseller dan pembeli. Dan Bahasa pemrograman yang digunakan adalah PHP dan HTML.</p>

<li><strong>3.6	Model Proses</strong></li>
<p>Untuk menggambarkan pemodelan proses digunakan DFD (Data Flow Diagram), yang untuk masing- masing level akan digambarkan sebagai berikut:</p>
<p>DFD Level 0 (Context Diagram)<p>
<p>Dalam perancangan DFD level 0, entitas eksternal yang terlibat adalah:</p>
<ol>
	<li>Penjual </li>
	<li>Admin</li>
	<li>Pembeli</li>
</ol>


