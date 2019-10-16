#Latihan 1

Menambahkan Global Config

Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user.name dan user.email

• konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository. 

• apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit

 config Global Repository 

    $ git config --global user.name “nama_user” 
    $ git config --global user.email “nama_user”

Membuat Reposiory Local

Buka direktory aktif, misal: c:\user\iip\lab_pemrograman (buka menggunakan Windows Explorer)

klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash command

Buat direktory project praktikum pertama dengan nama latihan1

    $ mkdir latihan1 $ cd latihan1

Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory) 

• direktory aktif menjadi: c:\user\iip\lab_pemrograman\latihan1

Jalankan perintah git init, untuk membuat repository local. 

    $ git init

Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

Pada direktori tersebut, semua perubahan pada working directory akan disimpan.

Menambahkan File baru pada repository

Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

disini kita akan coba buat satu file bernama README.md (text file) 

    $ echo “#Latihan 1” >> README.md

![l2](https://user-images.githubusercontent.com/44857690/66886035-51875280-f000-11e9-84dc-6679cdef613a.png)

![lat1 1](https://user-images.githubusercontent.com/44857690/66886036-51875280-f000-11e9-91de-152a76a254b2.PNG)

File README.md berhasil dibuat.

Menambahkan File baru pada repository

Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add. 

$ git add README.md

File README.md berhasil ditambahkan. Github 2

Commit (Menyimpan perubahan ke database)

Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit” 

$ git commit -m “File pertama saya”

Perubahan berhasil disimpan. 

Membuat repository server

Server reopsitory yang akan kita gunakan adalah http://github.com • Anda harus membuat akun terlebih dahulu.

Pada laman github, klik tombol start a project, atau

Dari menu (icon +) klik New Repositori.

Isi nama repositorynya, misal: lab_prog1.

lalu klik tombol Create repositor.

Menambahkan Remote Repository

Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]

    $ git remote add origin https://github.com/itsrifki/lab_prog1

Push (Mengirim perubahan ke server)

Untuk mengirim perubahan pada local repository ke server gunakan perintah git push. 

    $ git push -u origin master

Perintah ini akan meminta memasukkan username dan password pada akun github.com 

Melihat hasilnya pada server repository

Buka laman github.com, arahkan pada repositorinya.

Maka perubahan akan terlihat pada laman tersebut. Github 7

Clone Repository

Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

Untuk melakukan cloning, gunakan perintah git clone [url] Github 8
