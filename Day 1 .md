# Day 1
## Definisini DevOps
DevOps adalah pendekatan dalam pengembangan perangkat lunak dan manajemen infrastruktur yang bertujuan untuk mengatasi kesenjangan antara tim pengembangan (development) dan tim operasi (operations) dalam siklus hidup perangkat lunak. Tujuan utamanya adalah untuk meningkatkan efisiensi, kecepatan, dan kualitas dalam pengembangan, pengujian, pengiriman, dan operasi perangkat lunak.

## Siklus Hidup DevOps
Siklus hidup DevOps melibatkan serangkaian praktik dan konsep yang dikenal sebagai "Continuous" (Berkelanjutan). Berikut adalah beberapa fase utama dalam siklus hidup DevOps beserta definisi-definisinya:

1. **Continuous Integration (CI)**:
   CI adalah praktik di mana anggota tim pengembangan secara teratur menggabungkan kode yang mereka hasilkan ke dalam repositori bersama. Setiap kali ada perubahan kode, otomatisasi akan memicu proses pengujian otomatis untuk memastikan bahwa perubahan tersebut tidak mempengaruhi fungsionalitas eksisting dan memenuhi standar kualitas tertentu.

2. **Continuous Delivery (CD)**:
   CD melibatkan otomatisasi dalam proses penerbitan dan pengiriman perangkat lunak yang siap untuk dipasang ke lingkungan produksi. Dengan CD, perangkat lunak yang telah melalui fase pengujian CI dijalankan melalui serangkaian pengujian lebih lanjut, termasuk pengujian fungsional dan pengujian performa, sebelum siap untuk diterapkan.

3. **Continuous Deployment (CD)**:
   Continuous Deployment adalah perpanjangan dari Continuous Delivery. Dalam praktik ini, setiap kali perubahan kode lulus pengujian dan memenuhi persyaratan kualitas, perubahan tersebut secara otomatis diterapkan ke lingkungan produksi tanpa campur tangan manusia.

4. **Continuous Monitoring (CM)**:
   Continuous Monitoring melibatkan pemantauan berkelanjutan terhadap lingkungan produksi, kinerja perangkat lunak, dan infrastruktur. Hal ini membantu mendeteksi masalah dengan cepat dan memungkinkan tim untuk merespons ancaman atau masalah potensial dalam waktu nyata.

5. **Continuous Feedback**:
   Continuous Feedback melibatkan umpan balik berkelanjutan dari pelanggan, pengguna, dan lingkungan produksi. Informasi ini digunakan untuk terus meningkatkan perangkat lunak, mengidentifikasi peluang perbaikan, dan merespons kebutuhan yang berkembang.

6. **Continuous Improvement (CI)**:
   Continuous Improvement adalah siklus berkelanjutan dalam upaya untuk meningkatkan proses pengembangan dan pengiriman perangkat lunak. Tim terus menerapkan perbaikan berdasarkan hasil pemantauan, umpan balik, dan evaluasi kinerja.

7. **Continuous Testing (CT)**:
   Continuous Testing adalah praktik memastikan bahwa pengujian perangkat lunak berlangsung sepanjang siklus pengembangan dan pengiriman. Ini mencakup pengujian fungsional, integrasi, performa, keamanan, dan lebih banyak lagi.

Dengan menggabungkan semua elemen ini, siklus hidup DevOps menciptakan alur kerja yang berkesinambungan, di mana perubahan kode dikelola dengan baik, diuji secara otomatis, dan diintegrasikan ke dalam lingkungan produksi secara cepat dan aman. Ini memungkinkan organisasi untuk mencapai pengiriman perangkat lunak yang lebih cepat, lebih handal, dan lebih adaptif terhadap perubahan bisnis dan kebutuhan pelanggan.

## Cara instalasi Ubuntu Server
1.	Klik Create a new virtual machine (karna VM Ware saya tidak bisa maka saya menggunakan VirtualBox) 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(49).png?raw=true)
2.	Kemudian masukan nama serta ganti typenya menjadi Linux dan versinya Ubuntu (64-bit)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(50).png?raw=true)
3.	Ganti ukuran  memori menjadi 1 GB (1024 MB)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(51).png?raw=true)
4.	Pilih yang  buat hard disk virtual sekarang lalu klik
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(52).png?raw=true)
5.	Kemudian untuk buat hard disk virtual pilih yang VDI (VirtualBox disk Image)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(53).png?raw=true)
6.	Sesudah itu pilih yang dialokasikan secara dinamik
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(54).png?raw=true)
7.	Lalu buat ukurannya menjadi 20 GB
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(55).png?raw=true)
8.	Nanti akan menjadi seperti ini. Habis itu klik yang pengaturan
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(56).png?raw=true)
9.	Abis itu pilih yang jaringan
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(57).png?raw=true)
10.	Kemudian ganti dari NAT ke Adaptor Ter-Bridge  klik oke dan klik mulai.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(58).png?raw=true)
11.	Kemudian ketika sudah klik mulai. Muncul seperti ini dan pilih bahasa yang diinginkan
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(60).png?raw=true)
12.	Nanti akan muncul seperti ini dan klik saja continue without update
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(61).png?raw=true)
13.	Dari sini klik done saja
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(62).png?raw=true)
14.	Nanti akan masuk ke jaringan lalu pilih yang enpose eth
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(63).png?raw=true)
15.	Lalu klik edit IPv4
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(64).png?raw=true)
16.	kemudian muncul seperti ini dan klik manual 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(65).png?raw=true)
17.	Nanti akan muncul seperti ini dan isi sesuai dengan ip masing-masing. Cara melihat ip bisa buka di search windows abis itu ketik cmd maka akan muncul bentuk cmdnya. Sesudah itu ketik ipconfig. dana akan muncul ipconfignya. jika sudah maka klik save.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(66).png?raw=true)
18.	Jika sudah beres maka klik done. Tapi jika ada tulisan continue without network, maka ada yang salah dengan ip nya dan perbaiki kembali
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(67).png?raw=true). 
19.	Jika sudah maka klik saja done sampai ke custom storage  layout lalu centang dan klik done. 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(70).png?raw=true)
20.	Jika sudah maka akan muncul seperti ini lalu kli yang free space lalu pilih yang Add GPT partition. 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(71).png?raw=true)
21.	Lalu jika muncul seperti ini, bebas mau isi berapa Giga. Hanya saja usahakan isinya 15 Giga karna untuk menaruh file yang storagenya lebih banyak lalu klik create.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(72).png?raw=true)
22.	Pilih kembali ke free space lalu pilih yang Add  GPT partition.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(74).png?raw=true)
23.	Karna ada sisa 4G kita buat untuk swap. Swap ini berfung jika file yang 15G penuh maka swap bisa menjadi pengganti untuk sementara agar tidak menjadi hang perangkatnya. Sesudah itu klik create.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(75).png?raw=true)
24.	Lalu akan muncul ditampilan seperti ini dan klik done.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(76).png?raw=true)
25.	Ketika sudah mengklik done maka akan muncul seperti ini. Ini adalah peringatan bahwa nanti tidak akan bisa kembali ke setingan. Jika sudah yakin maka klik continue.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(77).png?raw=true)
26.	Isi biodatanya. 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(78).png?raw=true)
27.	Centang install OpenSSH Server lalu klik done
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(79).png?raw=true)
28.	Klik continue. 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(80).png?raw=true)
29.	Jika ada tampilan seperti ini lewatkan saja dan klik done. 
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(81).png?raw=true)
30.	Maka install sudah dimulai dan mungkin memakan cukup waktu yang lama.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(82).png?raw=true)
31.	Jika sudah di install maka akan muncul tampilan seperti ini lalu klik reboot now.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(83).png?raw=true)
32.	Isi username serta password yang sudah dibuat tadi
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(84).png?raw=true)
33.	Dan Ubuntu siap digunakan.
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(85).png?raw=true)