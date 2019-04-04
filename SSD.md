<p align="center"><font size="5"><b>SOFTWARE DESIGN DOCUMENT</b></font><br>
	<font size="5"><b>APLIKASI PENJUALAN OLAHAN</b></font><br>
	<font size="5"><b>BUAH MANGGA INDRAMAYU BERBASIS WEBSITE</b></font><br></p>

<p align="center"><img src="Gambar/POLINDRA.png" width="250" height="250"></p>

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

