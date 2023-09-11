# Day 2 Week 2 Manage Server In Terminal
## Manage Server In Terminal
Manage Server In Terminal adalah meanipulasi pada file menggunakan terminal, tanpa menggunakan teks editor seperti nano

### *Cat*
*Cat* adalah salah satu perintah yang berfungsi untuk membuat daftar konten atau isi file pada standard output (sdout). Yang kita tahu pasti perintah *cat* hanya bisa untuk melihat isi dari suatu file, tetapi bisa melakukan hal lain.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(145).png?raw=true)
```.
cat > filezulfi
```
Lalu ketik kata atau kalimat yang diinginkan
```
cat filezulfi
```
Kita bisa menggabungkan kedua file beserta isinya
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(146).png?raw=true)
```
cat > filealfain
```
Lalu buat kata atau kalimat yang diinginkan
```
cat filezulfi filealfain > filerahman
```
```
cat filerahman
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(147).png?raw=true)

### *Sed*
*Sed* adalah singkatan dari system editor. Yang berguna untuk memanipulasi teks dasar pada file. Dengan *sed* kita bisa mengganti teks dengan cepat.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(147).png?raw=true)
```
sed -i 's/Hallo/Hola/g' filerahman
```

### *Grep*
*Grep* adalah perintah untuk melakukan pencarian sebuah text dalam sebuah file yang telah tadi kita buat.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(148).png?raw=true)
```
grep Zulfikar filerahman
```
Bisa juga kita mencari teks dalam file yang tertentu
```
grep -c Zulfikar filerahman
```
Bisa juga menghitung jumlah teks yang ada di dalam file
```
grep Zulfikar *
```
Berfungsi mencari tek dalam semua file

### *Sort*
*Sort* adalah perintah untuk mengurutkan data, baik itu secara ascending atau descending.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(149).png?raw=true)
```
cat > filenomor
```
Membuat file yang berisi text acak
```
sort filenomor
```
Mengurutkan text dari yang terkecil sampai yang terbesar
```
sort -r filenomor
```
Mengurutkan text dari yang terbesar sampai yang terkecil

### *Echo*
*Echo* adalah perintah yang digunakan untuk mencetak string atau pesan dari hasil perintah yang lain.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(150).png?raw=true)
```
echo "zulfikar alfain"
```
Berfungsi untuk mencetak kata atau kalimat
```
echo "zulfikar alfain" >> zulfikaralfainfile
```
berfungsi untuk mencetak data zulfikar alfain pada zulfikaralfainfile
```
echo "hai zulfikar" > zulfikaralfainfile
```
Berfungsi untuk mengganti semua data zulfikaralfainfile dengan Hai Zulfikar

## Penjelasan tool htop atau nmon
### *Htop*
*Htop* adalah perintah untuk memonitoring sistem, kita bisa melihat penggunaan memory,cpu,swap.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(151).png?raw=true)
```
sudo apt install htop -y
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(152).png?raw=true)
```
htop
```

## BASH Script untuk instalasi nginx
####  Buat file script.sh
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(153).png?raw=true)
```
nano script.sh
```
#### Buat perintah seperti ini
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(154).png?raw=true)
```
#!/usr/bin/env bash

sudo apt install nginx
```
#### Jalankan scrip dengan perintah
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(154).png?raw=true)
```
sh script.sh
```
#### Kemudian buka web dan isi dengan IP masing-masing
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(155).png?raw=true)
```
192.168.2.123
```
