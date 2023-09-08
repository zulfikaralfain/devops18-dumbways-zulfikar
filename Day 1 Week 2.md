# Day 1 Week 2 Version Control System
## Distributed Version Control
Distributed Version Control (DVC) adalah suatu metode untuk mengelola perubahan dalam kode sumber atau proyek perangkat lunak dengan menggunakan sistem kontrol versi yang didistribusikan. DVC memungkinkan pengembang untuk bekerja dengan repositori kode sumber secara terdistribusi, artinya setiap pengembang memiliki salinan lengkap dari repositori secara lokal di komputernya. Ini berbeda dengan sistem kontrol versi terpusat, di mana ada satu repositori pusat yang digunakan sebagai sumber utama kode sumber. Contoh sistem kontrol versi yang didistribusikan yang populer adalah Git, Mercurial, dan Bazaar. Git, khususnya, telah menjadi salah satu yang paling banyak digunakan di seluruh dunia untuk mengelola proyek perangkat lunak, dan ini membantu mendorong adopsi DVC secara luas dalam pengembangan perangkat lunak modern.

## Buat Repository dengan memakai makanan kesukaan
### Membuat Repository melalui akun GitHub
Masuk ke akun GItHub lalu creat new repository (disini saya menggunakan nama pet)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(131).png?raw=true)

### Membuat repository menggunakan terminal
Beri perintah dari Git ini untuk inialisasi repository dengan Git
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(132).png?raw=true)
```
git init
```
### Buat berkas baru dan periksa berkas tersebut
Pengecekan status dari Repositori yang baru dibuat bisa dilihat melalui Git. Sekarang terdapat tiga berkas (file) yang tidak masuk dalam pengamatan (Untracked) dari Git yang dapat ditambahkan melalui perintah ```git add```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(133).png?raw=true)
```
touch sambal bakar tumis
```
```
git status
```
```
git add
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(136).png?raw=true)
### Buat perubahan baru (Commit)
Tulis pesan untuk setiap perubahan yang tadi dilakukan di repository
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(137).png?raw=true)
```
git commit -m "(disini bebas mau tulis pesan apapun)"
```
### Menaruh Remote (Link kendali) dari Github
Tambahkan Remote link untuk terhubung ke akses Repository melalui Github
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(138).png?raw=true)
```
git remote add origin git@github.com:zulfikaralfain/pete.git
```
```
git remote -v (jika ingin mengecek ulang tautan)
```
### Menerapkan perubahan ke repository Github
Jika sudah sesuai keinginan, lakukan *push* ke repository yang sudah di tautkan tersebut.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(139).png?raw=true)
```
git push origin master
```
### Menambahkan Branch (Ranting) di repository
Jika ada yang ingin menambah *branch* baru dapat menggunakan :
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(140).png?raw=true)
```
git branch (branch_name) # Ubah baris (branch_name) sesuai keinginan
```

## 3 (Tiga) Perintah Git
### *Git log*
 Menampilkan riwayat commit dalam repositori, termasuk pesan-pesan komit, penulis, waktu, dan hash SHA-1 yang unik untuk setiap komit.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(141).png?raw=true)
 
 ### *Git stash*
 Menyimpan perubahan yang belum selesai untuk sementara waktu sehingga Anda dapat beralih ke branch lain atau menyelesaikan tugas lain.
 ![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(142).png?raw=true)
 
 ### *Git blame*
 digunakan untuk menampilkan riwayat perubahan pada setiap baris dalam file.
 ![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(144).png?raw=true)