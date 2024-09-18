**LAPORAN PRAKTIKUM 5 SISTEM OPERASI**

1.  Lihat daftar secara lengkap pada direktori aktif, belokkan tampilan standard output ke file 
baru.
![Screenshot 2024-09-12 142819](https://github.com/user-attachments/assets/cf452638-5035-4776-943e-25cb049bba0a)

- Untuk melihat daftar direktori aktif, gunakan perintah $ ls
- sedangkan untuk membelokkan tampilan standard output ke file baru, gunakan ‘>’
- cat baru akan menampilkan isi dari file baru, hasilnya adalah daftar yang sama seperti yang ditampilkan oleh perintah ls sebelumnya, karena file baru telah diisi dengan output dari perintah ls.

2. Lihat daftar secara lengkap pada direktori /etc/paswd, belokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya.
![Screenshot 2024-09-12 143208](https://github.com/user-attachments/assets/72ab2b86-b990-405c-aae2-b0de24b7f5af)

- Untuk melihat daftar lengkap dari direktori /etc/passwd, gunakan perntah $ ls, sedangkan untuk membelokkan tampilan standard output ke file baru tanpa menghapus file baru sebelumnya, gunakan ‘>>’

3. Urutkan file baru dengan cara membelokkan standard input.
![Screenshot 2024-09-12 143320](https://github.com/user-attachments/assets/c8fab9ef-44e0-4322-82d1-c9d9a2b6e805)

- Untuk mengurutkan file, gunakan perintah sort, sedangkan gunakan ‘<’ untuk membelokkan standard input dari file baru ke perintah sort, sehingga perintah sort menerima isi file baru untuk diurutkan.

4.  Urutkan file baru dengan cara membelokkan standard input dan standard output ke file baru.urut.
![Screenshot 2024-09-12 143704](https://github.com/user-attachments/assets/51923bab-ccad-4218-a0db-592d006808cb)

- Gunakan perintah sort untuk mengurutkan file
- sedangkan untuk membelokkan standard input gunakan ‘<’
- untuk membelokkan standard output ke file, gunakan ‘>’
- Pembelokan standart input dan standart output dapat dikombinasikan asalkan tidak boleh menggunakan nama file yang sama sebagai standart input dan output

5. Buatlah direktori latihan2 sebanyak 2 kali dan belokkan standard error ke file rmdirerror.txt.
![Screenshot 2024-09-18 220017](https://github.com/user-attachments/assets/bcc0b08c-0963-4751-96eb-7f9a0fa5314c)

- Gunakan perintah mkdir untuk membuat direktori baru yaitu latihan6.  Saat membuat direktori yang sama sebanyak dua kali, akan muncul pesan error
- mkdir latihan6 2> rmdirerror.txt: Perintah ini mencoba lagi untuk membuat direktori latihan6. Karena direktori sudah ada, maka sistem mengeluarkan pesan error yang sama. Namun kali ini, pesan error diarahkan ke file rmdirerror.txt dengan simbol 2>, yang berarti bahwa standard error akan disimpan ke file tersebut.
- cat rmdirerror.txt: Perintah ini digunakan untuk menampilkan isi file rmdirerror.txt. Hasilnya adalah pesan error yang sama, yaitu "tidak dapat membuat direktori latihan6: Berkas telah ada", yang telah disimpan saat perintah ketiga dijalankan.

6. Urutkan kalimat berikut :  
Jakarta  
Bandung  
Surabaya  
Padang  
Palembang  
Lampung  
Dengan menggunakan notasi here document (<@@@ …@@@)
![6](https://github.com/user-attachments/assets/c5dc39d8-54c9-44d0-815b-8e279c0984ce)

- Buat notasi here document yang akan dibelokkan ke sebuah file kemudian isi document tersebut. Setelah diisi dan diakhiri, isi dokumen 
akan tersimpan ke file yang dibelokkan. File tersebut kemudian diurutkan menggunakan perintah sort.
- @@@ penanda akhir dari here document, yang menandai bahwa semua input telah dimasukkan.

7. Hitung jumlah baris, kata dan karakter dari file baru.urut dengan menggunakan filter dan tambahkan data tersebut ke file baru.
![7](https://github.com/user-attachments/assets/f7035a5b-c278-45c0-97e6-8423f741580e)

- Untuk mendapatkan jumlah baris, kata, dan karakter (secara berurutan) dari sebuah file, gunakan perintah wc yang dipipakan dengan perintah cat. Hasilnya kemudian bisa ditambahkan ke file menggunakan ‘>>’

8. Gunakan perintah di bawah ini dan perhatikan hasilnya. 
$ cat /etc/passwd | sort | pr –n | grep tty03  
$ find /etc –print | head  
$ head /etc/passwd | tail –5 | sort
![8](https://github.com/user-attachments/assets/81442f9c-7cb2-4e73-a901-23c18182188d)

- $ cat /etc/passwd | sort | pr -n | grep tty03
  Hasil yang diharapkan: Anda akan melihat baris dari file /etc/passwd yang berisi "tty03", jika ada, lengkap dengan nomor baris. Jika "tty03" tidak ditemukan, tidak akan ada output.
- $ find /etc -print | head
  Hasil yang diharapkan: Anda akan melihat 10 file atau direktori pertama yang ditemukan di dalam direktori /etc. Ini termasuk subdirektori dan file di dalamnya.
- $ head /etc/passwd | tail -5 | sort
  Hasil yang diharapkan: Anda akan melihat 5 baris terakhir dari 10 baris pertama file /etc/passwd, diurutkan secara alfabetis.
- Kesimpulannya adalah perintah pertama digunakan untuk mencari pengguna terkait terminal "tty03" di file /etc/passwd. Perintah kedua digunakan untuk menemukan dan menampilkan 10 file atau direktori pertama di dalam /etc dan perintah ketiga menampilkan dan mengurutkan 5 baris terakhir dari 10 baris pertama file /etc/passwd.

9. Gunakan perintah $ who | cat | cat | sort | pr | head | cat | tail dan perhatikan hasilnya. 
![9](https://github.com/user-attachments/assets/53706a7c-0eea-4645-93f7-87fd80dc5a60)

- who: Perintah ini menampilkan daftar pengguna yang sedang login ke sistem. Ini mencakup informasi seperti nama pengguna, terminal yang digunakan, dan waktu login.
- cat | cat: Dua kali penggunaan cat tidak mempengaruhi hasil. Perintah ini hanya meneruskan inputnya tanpa perubahan. Jadi output dari who tetap sama.
- sort: Mengurutkan output dari perintah who secara alfabetis (berdasarkan nama pengguna, jika ada).
- pr: Mengubah output yang telah diurutkan menjadi format halaman, dengan header dan nomor halaman.
- head: Menampilkan 10 baris pertama dari hasil yang telah di-format oleh pr.
- cat: Lagi-lagi hanya meneruskan output tanpa perubahan.
- tail: Menampilkan baris terakhir dari hasil head (dalam kasus ini, baris ke-10 dari output who).

Hasil akhir dari perintah ini adalah baris terakhir (baris ke-10) dari daftar pengguna yang sedang login, setelah melalui serangkaian operasi, termasuk pengurutan alfabetis dan pemformatan halaman. Jika ada kurang dari 10 pengguna yang sedang login, hasilnya adalah pengguna terakhir yang login (atau baris terakhir dari output who setelah diurutkan).
