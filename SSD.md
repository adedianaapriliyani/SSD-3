<p><strong>SOFTWARE DESIGN DOCUMENT</strong></p>
<p><strong>APLIKASI PENJUALAN </strong><strong>OLAHAN </strong></p>
<p><strong>BUAH MANGGA </strong><strong>INDRAMAYU BERBASIS WEBSITE</strong></p>
<p><strong>TIKB2293 PROYEK II </strong></p>
<p>Diajukan untuk Memenuhi Persyaratan Mata Kuliah Proyek II</p>
<p>&nbsp;</p>
<p><strong>&nbsp;</strong></p>
<p>Disusun Oleh:</p>
<p>Ade Diana Apriliyani&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (1703072)</p>
<p>Fany Fahrurozi&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (1703060)</p>
<p>Fiqi Andri Reviansyah&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (1703064)</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>D3 TEKNIK INFORMATIKA</strong></p>
<p><strong>POLITEKNIK NEGERI INDRAMAYU</strong></p>
<p><strong>&nbsp;</strong></p>
<p>Jl. Lohbener Lama No.08, Lohbener, Indramayu, Legok, Lohbener, Kabupaten Indramayu, Jawa Barat 45252, Indonesia</p>
<p><strong>&nbsp;</strong></p>
<h1><strong>KATA PENGANTAR</strong></h1>
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
<p><br /> <br /> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;Indramayu, 10 Februari 2019<br /> <br /> <br /> <br /> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Penulis<br /> </p>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>RINGKASAN </strong></p>
<p>Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website (MANGOLINESHP) adalah salah satu jenis aplikasi perangkat lunak yang dapat digunakan untuk membantu proses penjualan olahan secara online. Selama ini pemasaran olahan mangga khas Indramayu dipasarkan secara konvensional yaitu dijual di toko sekitar Indramayu saja. Pemasaran olahan mangga Indramayu pun kurang berkembang karena pembeli harus datang ke toko. Oleh karena itu olahan mangga&nbsp; khas Indramayu pun yang mengenal hanya orang-orang yang singgah atau berwisata ke Indramayu saja. Sehingga kami berinisiatif untuk membuat sebuah wadah yang didalamnya terdapat lapak-lapak penjual olahan mangga dalam bentuk aplikasi berbasis website. Dibuatnya aplikasi ini kami bisa membantu pemasaran dari penjual olahan mangga Indramayu serta mempromosikan tentang keberagaman olahan mangga yang ada di Indramayu.</p>
<p>Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website ini dibangun dengan menggunakan framework laravel dengan didukung basis data MYSQL.</p>
<p><strong>Kata kunci&nbsp;&nbsp;&nbsp;&nbsp; : </strong>Aplikasi Penjualan, framework laravel, MYSQL</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong><br /> </strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>BAB I</strong></p>
<p><strong>PENDAHULUAN</strong></p>
<ul>
<li><strong>Tujuan</strong></li>
</ul>
<p>Tujuan pembuatan SDD (Software Design Description) ini&nbsp;&nbsp; adalah untuk menjelaskan langkah langkah desain dan proses-proses dalam pembuatan sistem aplikasi yang akan diterapkan pada Aplikasi Mangolineshop (Aplikasi Penjualan Olahan Mangga Indramayu Berbasis Website), dan juga memberi definisi kebutuhan untuk sistem, spesifikasi kebutuhan fungsional.</p>
<p>Fungsi utama dari aplikasi Mangolineshop ini adalah mempermudah penjual olahan mangga dalam memberikan pelayanan terhadap pembeli, memudahkan penjual dalam rekap laporan keuangan, dan sebagai sarana untuk mempromosikan produk olahan mangga khas Kota Indramayu.</p>
<p>Secara ringkas, fungsi Aplikasi Mangolineshop dapat dituliskan sebagai berikut :</p>
<ol>
<li>Admin dapat menginputkan fitur kategori produk, akun penjual, dan akun pembeli yang nantinya akan digunakan oleh user dalam aplikasi tersebut.</li>
<li>Admin merekap laporan transaksi.</li>
<li>Aplikasi penjual harus mendaftar terlebih dahulu di admin Mangolineshop.</li>
<li>Aplikasi penjual dan admin login, kemudian memberikan detail produk olahan mangga pada pembeli.</li>
<li>Pembeli harus melakukan konfirmasi pembelian terlebih dahulu setelah memilih produk olahan mangga yang ingin dibeli pada aplikasi Manolineshop.</li>
<li>Pembeli melakukan pembayaran setelah konfirmasi pemesanan menu &ndash; menu yang dibeli di aplikasi kasir sebagai bukti pembayaran.</li>
<li>Aplikasi penjual dan admin login, kemudian melakukan proses perhitungan pembayaran untuk pembeli.</li>
<li>Setelah melakukan transaksi penjual dan admin dapat melihat laporan pendapatan terhadap pemesanan yang dilakukan oleh pembeli.</li>
</ol>
<p>&nbsp;</p>
<ul>
<li><strong>Ruang Lingkup</strong></li>
</ul>
<p>Hasil dari SDD ini adalah aplikasi yang berbasis web, yang digunakan untuk membantu pemasaran dan pengelolaan yang ada di UKM Kenanga Mandiri dalam hal :</p>
<ol>
<li>Mencatat produk olahan mangga Indramayu yang akan ditampilkan di aplikasi Mangolineshop.</li>
<li>Mencatat pemesanan produk olahan mangga terhadap pembeli di aplikasi Mangolineshop.</li>
<li>Menghitung transaksi terhadap pemesanan yang dilakukan oleh pembeli yang akan dilakukan pada aplikasi Admin dari aplikasi Mangolineshop.</li>
<li>Mencatat laporan transaksi yang akan ditampilkan di aplikasi penjual dan admin dari aplikasi Mangolineshop.</li>
</ol>
<ul>
<li><strong>Gambaran umum dokumen</strong></li>
</ul>
<p>Penulisan dokumen ini dibagi menjadi beberapa bab sebagai berikut:</p>
<ol>
<li>Bab 1, adalah Pendahuluan yang menjelaskan mengenai tujuan perangkat lunak, ruang lingkup, serta gambaran umum dokumen.</li>
<li>Bab 2, adalah Deskripsi Umum, yang berisi tentang gambaran umum mengenai perspektif produk, manfaat produk, karakteristik user dan stakeholder, batasan, serta asumsi dan ketergantungan yang digunakan.</li>
<li>Bab 3, adalah Software Design, yang menyediakan spesifikasi, kebutuhan, antarmuka, kebutuhan fungsional dan nonfunctional, lingkungan operasi, dan batasan perancangan, permodelan proses, permodelan data, struktur data, spesifikasi program dan desain interface.</li>
</ol>
<p>&nbsp;</p>
<p><strong>BAB II</strong></p>
<p><strong>DESKRIPSI UMUM</strong></p>
<p><strong>&nbsp;</strong></p>
<p><strong>2.1 Perspektif Produk</strong></p>
<p>Produk dari SDD ini adalah sebuah aplikasi yang berbasis web, yang akan dijalankan dan berfungsi sebagai untuk mempermudah layanan penjualan olahan mangga, seperti yang telah dijelaskan pada Pendahuluan. Produk ini akan dapat diakses dari browser yang berjalan pada sistem operasi Windows maupun Linux.</p>
<p><strong>2.2 Manfaat Produk</strong></p>
<p>Manfaat yang didapat manajemn dalam menggunakan siste atau aplikasi Mangolineshop ini adalah:</p>
<ol>
<li>Memudahkan proses pemesanan produk olahan mangga Indramayu bagi pe</li>
<li>Memudahkan admin dan penjual dalam melakukan perhitungan</li>
<li>Memudahkan penjual memantau penjualan pada aplikasi Mangolineshop.</li>
<li>Menyediakan informasi mengenai produk olahan mangga Indramayu kepada pembeli.</li>
</ol>
<p><strong>2.3 Karakteristik User dan Stakeholder User</strong></p>
<ol>
<li>Yang terlibat adalah sebagai berikut :</li>
<li>Admin</li>
<li>Penjual</li>
<li>Reseller</li>
<li>Pembeli</li>
<li>Stakeholder yang terkait dengan system ini:</li>
<li>Mitra Kenanga Mandiri.</li>
<li>Kelompok Aplikasi Mangolineshop.</li>
</ol>
<p><strong>2.4 Batasan &ndash; Batasan</strong></p>
<ol>
<li>Aplikasi ini mencakup sistem pada admin dan penjual saja</li>
<li>Transaksi pembayaran langsung dilakukan pembeli dan kasir, sistem hanya membantu menampilkan transaksi yang dilakukan</li>
</ol>
<p><strong>2.5&nbsp;Asumsi</strong></p>
<ol>
<li>Setiap pembeli dapat langsung memesan produk melalui website yang ada pada aplikasi Mangolineshop.</li>
<li>Setiap penjual mempunyai username dan password yang diberikan oleh admin.</li>
</ol>
<p>Tersedia sarana koneksi ke internet, sarana jaringan komputer, dan sarana penunjang lainnya</p>