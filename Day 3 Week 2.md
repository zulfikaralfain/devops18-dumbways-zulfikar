# Day 2 Week 3 Web Server & Reverse Proxy
# Web Server & Reverse Proxy
## Buat 1 VM tambahan untuk nginx saja (Opsional)
Melakukan manipulasi pada sebuah file menggunakan terminal, tanpa menggunakan teks editor seperti nano.
### Membuat 1 VM ubuntu seperti minggu pertama (ssh baru "alfain")
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(157).png?raw=true)
### Melakukan update dan upgrade, dengan menulis perintah di bawah ini.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(158).png?raw=true)
```
sudo apt update; sudo apt upgrade
```
### Selanjutnya coba untuk menginstall aplikasi Nginx.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(159).png?raw=true)
```
sudo apt install nginx
```
### Cek dengan menggunakan perintah seperti ini
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(160).png?raw=true)
```
sudo systemctl status nginx
```
### Diusahakan buka browser kalian, lalu masukkan IP dari server kalian
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(162).png?raw=true)
```
192.168.2.234
```
## 2. menjalankan aplikasi Dumbflix menggunakan PM2
### Install PM2 dengan perintah sebagai berikut
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(163).png?raw=true)
```
npm install pm2 -g
```
### Masuk pada direktori src pada Dumbflix lalu jalankan PM2
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(164).png?raw=true)
```
cd src/
```
```
pm2 start index.js
```
## 3. Buatlah reverse proxy dengan directory /etc/nginx/dumbways
### Masuk ke folder nginx setelah itu buat suatu directory baru telebih dahulu
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(165).png?raw=true)
```
cd /etc/nginx
```
```
sudo mkdir dumbways
```
### Selanjutnya keluar dari directory dumbways, setelah itu masuk ke dalam file nginx.conf
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(166).png?raw=true)
```
sudo nano nginx.conf
```
### Selanjutnya pergi ke-bagian include, setelah itu masukan lokasi dari directory yang bersi konfigutasi yang sudah dibuat tadi
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(166).png?raw=true)
```
include /etc/nginx/dumbways/*;
```
## 4. Dengan menggunakan nginx, pastikan dumbflix bisa diakses ke domain yang diinginkan
### Setelah itu masuk ke directory yang sudah dibuat, setelah itu buat suatu file dengan nama dumbflix.conf
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(167).png?raw=true)
```
cd dumbways/
```
```
sudo nano dumbflix.conf
```
### Setelah itu masukkan konfigurasi berikut
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(167).png?raw=true)
```
server { 
    server_name dumbflix.xyz; 
  
    location / { 
             proxy_pass http://127.0.0.1:3000;
    }
}
```
### Setting host pada windows
pertama buka file explorer
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(168).png?raw=true)
```
C:\Windows\System32\drivers\etc
```
### Buka file host menggunakan administrator notepad
lalu pada bagian paling bawah tambahkan ip address dan domain yang sudah di configurasi pada server
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(168).png?raw=true)
```
192.168.2.123 dumbflix.xyz
```
### Pastikan untuk melakukan pengecekan konfigurasi dengan menjalankan perintah :
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(169).png?raw=true)
```
sudo nginx -t
```
### Jika sudah sekarang tinggal melakukan reload dan mengecek status Nginx
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(170).png?raw=true)
```
sudo systemctl reload nginx
```
```
sudo systemctl status nginx
```
### Sekarang coba buka web browser kalian setelah itu coba akses nama domain kalian
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(171).png?raw=true)

### Jalankan npm start pada direktori dumbflix-frontend
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(172).png?raw=true)