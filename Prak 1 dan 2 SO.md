# LAPORAN PRAKTIKUM
## PROSES INSTALASI SISTEM OPERASI LINUX

**Disusun oleh:**  
Nama: Fitria Dwi Handayani  
NIM: 09011282328105  
Kelas: SK3C  
Dosen Pengampu: Adi Hermansyah, M.T.

**PROGRAM STUDI SISTEM KOMPUTER**  
FAKULTAS ILMU KOMPUTER  
UNIVERSITAS SRIWIJAYA  
2024  

---

# BAB I  
## PENDAHULUAN

### 1.1 Latar Belakang
Sistem Operasi komputer adalah perangkat lunak komputer atau software yang bertugas untuk melakukan kontrol dan manajemen perangkat keras dan juga operasi-operasi dasar sistem, termasuk menjalankan software aplikasi seperti program-program pengolah data yang bisa digunakan untuk mempermudah kegiatan manusia. Pada saat ini hampir semua orang menggunakan sistem operasi Windows sebagai sistem operasi di komputer mereka. Namun, sudah tahukah Anda dengan Sistem Operasi Linux? Memang tak bisa dipungkiri bahwa sebagian besar masyarakat Indonesia masih mengalami kesulitan dalam menguasai teknologi. Hanya sebagian kecil yang memiliki pemahaman mendalam tentang IT.

### 1.2 Tujuan Praktikum
Untuk mengetahui cara menginstal Ubuntu berbasis Linux

### 1.3 Bahan dan Alat Praktikum
- Komputer/Pc/Laptop
- CD Linux

---

# BAB II  
## PEMBAHASAN

### 2.1 Pengertian Sistem Operasi
Sistem operasi atau operating system adalah kumpulan program yang bertugas mengelola sumber daya perangkat keras komputer dan menyediakan layanan umum untuk aplikasi perangkat lunak. Sistem operasi merupakan jenis perangkat lunak sistem yang paling penting dalam sebuah komputer. Tanpa sistem operasi, pengguna tidak akan bisa menjalankan program aplikasi di komputer mereka, kecuali program booting. Beberapa contoh sistem operasi modern termasuk Linux, Android, iOS, Mac OS X, dan Microsoft Windows. Secara umum, sistem operasi adalah perangkat lunak yang pertama kali dimuat ke dalam memori komputer saat komputer dinyalakan atau melakukan booting.

### 2.2 Pengertian Linux
Linux atau GNU/Linux adalah sistem operasi yang bebas dan sangat populer untuk digunakan pada komputer. Istilah ini sering merujuk pada keseluruhan distribusi Linux (Linux distribution), yang mencakup berbagai program pendukung sistem operasi. Linux merupakan contoh utama dari hasil pengembangan perangkat lunak yang bebas dan sumber terbuka. Seperti halnya perangkat lunak bebas dan sumber terbuka lainnya, kode sumber Linux dapat dimodifikasi, digunakan, dan didistribusikan kembali oleh siapa saja tanpa batasan.

### 2.3 Pengertian Ubuntu
Ubuntu adalah salah satu distribusi Linux yang berbasis pada Debian dan disebarkan sebagai perangkat lunak open source. Nama Ubuntu diambil dari sebuah filosofi Afrika Selatan yang berarti "kemanusiaan kepada sesama." Ubuntu dirancang untuk penggunaan pribadi, tetapi juga tersedia dalam versi server yang telah digunakan secara luas.

### 2.4 Langkah-langkah Instalasi Sistem Operasi Linux
1. Masukkan DVD Ubuntu 14.04 LTS installer (download di [http://releases.ubuntu.com/14.04/](http://releases.ubuntu.com/14.04/)) yang sudah di-burn dalam DVD. Sebelumnya, atur di BIOS untuk pengaturan booting dengan DVD-ROOM sebagai primer pertama booting. Tunggu hingga proses booting sampai keluar tampilan.
2. Pilih bahasa instalasi dan bahasa sistem operasi, kemudian pilih opsi "Install Ubuntu" untuk memulai proses instalasi.
3. Atur pengaturan jaringan jika diperlukan dan klik "Continue."
4. Pilih jenis instalasi, biasanya Anda dapat memilih "Erase disk and install Linux Mint" jika ini adalah instalasi bersih. Jika Anda menginstal bersama sistem operasi lain, pilih opsi yang sesuai.
5. Masukkan informasi pengguna seperti nama Anda, nama komputer, nama pengguna, dan password. Klik "Continue."
6. Tunggu hingga proses instalasi selesai. Proses ini memakan waktu beberapa menit. Setelah selesai, Anda akan diminta untuk me-restart mesin virtual.
7. Setelah restart, login ke Linux Mint menggunakan username dan password yang telah Anda buat.
8. Setelah semua proses instalasi selesai, Anda sekarang dapat mulai menggunakan Linux Mint.

---

# BAB III  
## ANALISA 

### 3.1 Hasil Instalasi
Berikut adalah tampilan apabila proses instalasi Linux sudah selesai dan komputer sudah di-restart. Setelah proses instalasi Linux selesai dan komputer di-restart, Anda akan disambut dengan layar login dari sistem operasi Linux yang baru saja Anda pasang. Pada layar ini, Anda akan diminta untuk memasukkan password yang telah Anda tetapkan selama proses instalasi. Password ini adalah kunci untuk mengakses akun pengguna Anda dan memulai sesi di sistem Linux. Setelah Anda memasukkan password yang benar, Anda akan diarahkan ke desktop environment atau command line interface, tergantung pada distribusi dan konfigurasi yang Anda pilih. Jika Anda menginstal Linux dalam lingkungan virtual, seperti menggunakan VirtualBox atau VMware, langkah-langkahnya serupa. Anda akan melihat jendela login virtual di mana Anda harus memasukkan password yang sama untuk masuk ke sistem operasi di dalam mesin virtual tersebut. Setelah berhasil login, Anda akan dapat menjelajahi dan mulai menggunakan berbagai fitur dan aplikasi yang tersedia di Linux.

![Alt Text](https://github.com/fitriadwiii/Fitria-Dwi-Handayani-09011282328105-SK3C/blob/main/GALERI/Screenshot%202024-08-29%20152124.png)
![Alt Text](https://github.com/fitriadwiii/Fitria-Dwi-Handayani-09011282328105-SK3C/blob/main/GALERI/Screenshot%202024-08-29%20143816.png)

### 3.2 Alasan Kenapa pada Saat Instalasi Perlu Dipilih “/” pada Opsi Mount Point
Alasan kenapa pada saat instalasi perlu dipilih “/” pada opsi Mount Point adalah karena simbol “/” merepresentasikan root directory, yang merupakan direktori utama dari seluruh sistem berkas pada Linux. Root direktori ini adalah tempat awal dimana nantinya semua direktori akan bercabang. Semua file dan direktori lainnya berada di bawah root ini. Menentukan "/" sebagai mount point berarti Anda mengatur tempat di mana sistem operasi akan diinstal dan dijalankan. Dengan demikian, sistem tahu di mana semua file sistem penting akan disimpan dan diakses.

### 3.3 Penjelasan tentang ext4, ext3, swap, ntfs, fat32, btrfs
- **Ext4 (4rd Extended):**  
  Ext4 atau Fourth Extended Filesystem adalah sistem file yang digunakan secara luas di Linux, sebagai penerus Ext3 dengan peningkatan signifikan dalam kinerja, keandalan, dan kapasitas penyimpanan. Ext4 mendukung ukuran file hingga 16 terabyte dan partisi hingga 1 exabyte, serta fitur-fitur seperti extent-based storage yang mengurangi fragmentasi, delayed allocation yang meningkatkan efisiensi, dan journaling yang menjaga integritas data. Selain itu, Ext4 memiliki kompatibilitas ke belakang dengan Ext3, memungkinkan pengguna untuk menggunakannya dengan lebih fleksibel tanpa kehilangan data.
  
- **Ext3:**  
  EXT3 adalah peningkatan dari EXT2 file sistem. Peningkatan ini memiliki beberapa keuntungan diantaranya, setelah kegagalan sumber daya, "unclean shutdown", atau kerusakan sistem, EXT2 file sistem harus melalui proses pengecekan dengan program e2fsck. Proses ini dapat membuang waktu sehingga proses booting menjadi sangat lama, khususnya untuk disk besar yang mengandung banyak sekali data. Dalam proses ini, semua data tidak dapat diakses. Jurnal yang disediakan oleh EXT3 menyebabkan tidak perlu lagi dilakukan pengecekan data setelah kegagalan sistem. EXT3 hanya dicek bila ada kerusakan hardware seperti kerusakan hard disk, tetapi kejadian ini sangat jarang. Waktu yang diperlukan EXT3 file sistem setelah terjadi "unclean shutdown" tidak tergantung dari ukuran file sistem atau banyaknya file, tetapi tergantung dari besarnya jurnal yang digunakan untuk menjaga konsistensi.

- **Swap:**  
  Swap pada Linux adalah ruang pada hard drive yang digunakan sebagai memori virtual tambahan ketika RAM (Random Access Memory) fisik pada sistem sudah penuh. Swap dapat berupa partisi khusus atau file swap. Ketika RAM tidak cukup untuk menangani semua proses yang sedang berjalan, sistem operasi akan memindahkan sebagian data dari RAM ke swap, sehingga membebaskan RAM untuk tugas lainnya. Meskipun swap lebih lambat dibandingkan RAM karena menggunakan hard drive, ini membantu mencegah crash sistem atau kehilangan data ketika memori fisik penuh. Swap juga dapat digunakan untuk mendukung fitur hibernasi, di mana seluruh isi RAM disimpan ke swap sebelum sistem dimatikan, sehingga bisa dilanjutkan nanti.

- **Ntfs:**  
  NTFS (New Technology File System) diperkenalkan pertama kali pada Windows NT dan merupakan file system yang benar-benar berbeda dibanding teknologi FAT. NTFS menawarkan security yang jauh lebih baik, kompresi file, cluster, dan bahkan support enkripsi data. NTFS merupakan file system standar untuk Windows XP dan apabila Anda melakukan upgrade Windows biasa, Anda akan ditanyakan apakah ingin mengupgrade ke NTFS atau tetap menggunakan FAT. Namun, jika Anda sudah menggunakan NTFS akan muncul masalah jika ingin downgrade ke FAT tanpa kehilangan data.

- **Fat32:**  
  FAT 32 (File Allocation Table 32) mulai dikenal pada sistem Windows 95 SP2, dan merupakan pengembangan lebih dari FAT16. FAT32 menawarkan kemampuan menampung jumlah cluster yang lebih besar dalam partisi. Selain itu juga mengembangkan kemampuan harddisk menjadi lebih baik dibanding FAT16. Namun FAT32 memiliki kelemahan yang tidak dimiliki FAT16 yaitu terbatasnya Operating System yang bisa mengenal FAT32. Tidak seperti FAT16 yang bisa dikenali oleh hampir semua sistem operasi, namun itu bukan masalah apabila Anda menjalankan FAT32 di Windows XP karena Windows XP tidak peduli file system apa yang digunakan pada partisi.

- **Btrfs:**  
  B-Tree File System (BTRFS) Kadang singkatan ini juga di
