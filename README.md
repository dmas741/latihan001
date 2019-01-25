Apa itu Git?



•	Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.

•	Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.

•	Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.






Membuat Reposiory Local



•	Buka direktory aktif, misal: d:\labs_pemrograman1 (buka menggunakan Windows Explorer)

•	klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

•	Buat direktory project praktikum pertama dengan nama latihan1








	


•	Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya 
•	masuk kedalam direktori tersebut dengan perintah cd (change directory)

•	direktory aktif menjadi: d:\labs_pemrograman1\latihan1
 ![mkdir](https://user-images.githubusercontent.com/46736003/51724806-98f43a00-2091-11e9-8f23-01f6857ed2a9.png)



 Membuat Reposiory Local




•	Jalankan perintah git init, untuk membuat repository local.


 


•	Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

•	Pada direktori tersebut, semua perubahan pada working directory akan disimpan.
![git init](https://user-images.githubusercontent.com/46736003/51724861-e7a1d400-2091-11e9-8c6e-cd0faca8976d.png)


Menambahkan File baru pada repository




•	Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

•	disini kita akan coba buat satu file bernama README.md (text file)


$ echo “#Latihan 1” >> README.md

•	File README.md berhasil dibuat.
 
![readme md](https://user-images.githubusercontent.com/46736003/51725204-909cfe80-2093-11e9-921c-fa97bbe263e6.png)


Menambahkan File baru pada repository




•	Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.


$ git add README.md

•	File README.md berhasil ditambahkan.

![git add readme md](https://user-images.githubusercontent.com/46736003/51725235-bd511600-2093-11e9-9bb7-44ca2f9f4a02.png)


Commit (Menyimpan perubahan ke database)




•	Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m “komentar commit”


$ git commit -m “File pertama saya”

•	Perubahan berhasil disimpan.
 
![git commit](https://user-images.githubusercontent.com/46736003/51725268-eb365a80-2093-11e9-866b-f979dd2fbc77.png)



Membuat repository server






•	Isi nama repositorynya, misal: latihan001.

•	lalu klik tombol Create repository
 
![create new repository](https://user-images.githubusercontent.com/46736003/51724531-5f6eff00-2090-11e9-948e-e2b6fd154cc8.png)



Menambahkan Remote Repository




•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah Menambahkan Remote Repository




•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]
![git remote add origin](https://user-images.githubusercontent.com/46736003/51724577-9ba25f80-2090-11e9-8cbc-e0bca2f45d20.png)

•	Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.


$ git push -u origin master

•	Perintah ini akan meminta memasukkan username dan password pada akun github.com
![git push](https://user-images.githubusercontent.com/46736003/51724609-cb516780-2090-11e9-90a9-ce91eda40f04.png)

Melihat hasilnya pada server repository



Buka laman github.com, arahkan pada repositorynya , maka perubahan akan terlihat pada laman tersebut.

![hasil repository](https://user-images.githubusercontent.com/46736003/51725413-91826000-2094-11e9-8be4-ec05c54526d4.png)

Clone Repository




•	Clone repository, pada dasarnya adalah meng-copy repository server dan secara otomatis membuat satu direktory sesuai dengan nama repositorynya (working directory).

•	Untuk melakukan cloning, gunakan perintah git clone [url]

![git clone](https://user-images.githubusercontent.com/46736003/51725433-b971c380-2094-11e9-9e37-17c2f4d80a51.png)
