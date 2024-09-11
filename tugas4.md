**LAPORAN PRAKTIKUM 4 SISTEM OPERASI**

1.  Lihat peralatan I/O, character device, yang ada pada system komputer.
![No 1](https://github.com/user-attachments/assets/aeec0983-f954-4fba-b17c-a9c1cdad4da0)
![No 1 (2)](https://github.com/user-attachments/assets/fc6ac63f-88e1-44c9-be20-48189d4854cc)

-  Perintah ini akan menampilkan daftar perangkat I/O (input/output) yang tersedia dalam direktori /dev. Setiap baris yang dimulai dengan huruf c menunjukkan file perangkat karakter (character device), yang merupakan antarmuka untuk perangkat yang mengirim atau menerima data dalam bentuk aliran karakter, seperti terminal (/dev/tty), printer, atau port serial.

2.	Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.
![No 2](https://github.com/user-attachments/assets/c9e2f4b4-3c5e-448e-962b-88b5aa9b0a00)
-	mkdir: Ini adalah perintah untuk membuat direktori baru (make directory).
-	 latihan5: Direktori utama yang akan dibuat. Jika direktori ini sudah ada, tidak akan dibuat ulang (kecuali dengan opsi tertentu seperti -p).
-	latihan5/januari, latihan5/februari, latihan5/maret: Subdirektori yang akan dibuat di dalam direktori latihan5. Direktori januari, februari, dan maret akan dibuat sebagai subdirektori dari latihan5.

3.	Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret.

![No 2 (2)](https://github.com/user-attachments/assets/9c4b76cb-dd0d-406f-9172-1a471aa777a0)
-	cd latihan5/januari: Perintah ini akan memindahkan Anda ke direktori januari, yang merupakan subdirektori dari latihan5.
-	perintah ini menggunakan echo untuk menambahkan informasi berupa "Nama", "NIM", dan "Alamat" ke dalam file dataku.txt.
-	simbol  >  menandakan bahwa teks yang dihasilkan oleh echo akan disimpan di dalam file dataku.txt.

![No 3](https://github.com/user-attachments/assets/4077068f-f8bb-41ad-b3c4-34cda212670f)
-	cp /home/dbake/latihan5/januari/dataku.txt /home/dbake/latihan5/februari: perintah ini akan menyalin file dataku.txt dari direktori januari ke direktori februari.

![No 3 (2)](https://github.com/user-attachments/assets/2ebe57c7-5c57-4594-8a2d-f198366307f2)
-	cp /home/dbake/latihan5/januari/dataku.txt /home/dbake/latihan5/maret: perintah ini akan menyalin file dataku.txt dari direktori januari ke direktori maret.

4.	Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.
![No 4](https://github.com/user-attachments/assets/98260a25-fb89-41ea-bb1f-5b0f9954cf34)
-	Perintah ini memberikan hak write (+w) kepada group dan others untuk file dataku.txt yang ada di dalam subdirektori januari.
-	Perintah ls -l akan menampilkan daftar file atau direktori beserta detail informasinya.

5.	Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute.
![No 5](https://github.com/user-attachments/assets/ddeeeb04-e1f1-4202-b3eb-1d585a7bf6f8)
-	chmod u+x,g-w,g+w,o+x dataku.txt: Menambahkan izin execute (+x) untuk pemilik (u) dan lainnya (o) dan menghapus izin write (-w) dari grup (g) dan menambah izin write (+w) untuk grup (g).
-	chmod g-w,g+w dataku.txt: Menghapus izin write (-w) dari grup (g), lalu menambah izin write (+w) untuk grup (g). 
Perintah kedua tidak mengubah izin karena operasinya bertentangan: pertama menghapus write dari grup, kemudian menambahkannya kembali.

6.	Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute.
![No 6](https://github.com/user-attachments/assets/1278e372-06de-4ff4-88bf-d7c2597aece6)
-	cd .. : Pindah ke direktori induk dari direktori saat ini.
-	cd maret: Masuk ke direktori maret.
-	ls -l: Menampilkan daftar file dan direktori beserta informasi izin aksesnya.
-	chmod 777 dataku.txt: Mengubah izin akses file dataku.txt sehingga semua pengguna (owner, group, others) dapat membaca, menulis, dan mengeksekusi file tersebut.
-	ls -l: Menampilkan daftar file dan direktori dengan informasi izin akses yang telah diperbarui.

7.	Hapuslah direktori maret.

![No 7](https://github.com/user-attachments/assets/e1a6a343-89e2-4a16-9f5b-3cdccb565ce9)
-	rm dataku.txt: Menghapus file dataku.txt dari direktori saat ini.
-	cd ..: Pindah ke direktori induk dari direktori saat ini.
-	rmdir maret: Menghapus direktori maret, tetapi hanya jika direktori tersebut kosong.
-	ls: Menampilkan daftar file dan direktori di direktori saat ini, untuk memverifikasi bahwa maret telah dihapus.

8.	Ubahkan kepemilikan sub direktori februari sehingga user dan group hanya dapat melakukan read, dan cobalah untuk membuat direktori baru haha pada sub direktori februari
![No 8](https://github.com/user-attachments/assets/0e99357b-ff7d-406c-bc49-5ecb04329cff)

9.	Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ?
![No 9](https://github.com/user-attachments/assets/a76309fb-1683-4b59-b476-2a02225ebc03)

10.	Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi ?

![No 10](https://github.com/user-attachments/assets/6e767ce8-9497-4159-b808-e6b568a20e8a)
