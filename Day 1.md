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
2.	Kemudian masukan nama serta ganti typenya menjadi Linux dan versinya Ubuntu (64-bit)
3.	Ganti ukuran  memori menjadi 1 GB (1024 MB)
4.	Pilih yang  buat hard disk virtual sekarang lalu klik itu
5.	Kemudian untuk buat hard disk virtual pilih yang VDI (VirtualBox disk Image)
6.	Sesudah itu pilih yang dialokasikan secara dinamik
7.	Lalu buat ukurannya menjadi 20 GB
8.	Nanti akan menjadi seperti ini. Habis itu klik yang pengaturan
9.	Abis itu pilih yang jaringan
10.	Kemudian ganti dari NAT ke Adaptor Ter-Bridge  klik oke dan klik mulai.
11.	Kemudian ketika sudah klik mulai. Muncul seperti ini dan pilih bahasa yang diinginkan
12.	Nanti akan muncul seperti ini dan klik saja continue without update
13.	Dari sini klik done saja
14.	Nanti akan masuk ke jaringan terus pilih yang enpose eth
15.	Lalu pilih yang manual
16.	Klik edit IPv4 
17.	Nanti akan muncul seperti ini dan isi sesuai dengan ip masing-masing. Cara melihat ip bisa buka di search windows abis itu ketik cmd maka akan muncul bentuk cmdnya. Sesudah itu ketik ipconfig 
18.	Jika sudah beres maka klik done. Tapi jika ada tulisan continue without network, maka ada yang salah dengan ip nya dan perbaiki kembali. 
19.	Jika sudah maka klik saja done sampai ke custom storage  layout lalu centang dan klik done. 
20.	Jika sudah maka akan muncul seperti ini lalu kli yang free space lalu pilih yang Add GPT partition. 
21.	Lalu jika muncul seperti ini, bebas mau isi berapa Giga. Hanya saja usahakan isinya 15 Giga karna untuk menaruh file yang storagenya lebih banyak lalu klik creat.
22.	Pilih kembali ke free space lalu pilih yang Add  GPT partition. 
23.	Karna ada sisa 4G kita buat untuk swap. Swap ini berfung jika file yang 15G penuh maka swap bisa menjadi pengganti untuk sementara agar tidak menjadi hang perangkatnya. Sesudah itu klik creat. 
24.	Lalu akan muncul ditampilan seperti ini dan klik done. 
25.	Ketika sudah mengklik done maka akan muncul seperti ini. Ini adalah peringatan bahwa nanti tidak akan bisa kembali ke setingan. Jika sudah yakin maka klik continue.
26.	Isi biodatanya. 
27.	Centang install OpenSSH Server lalu klik done 
28.	Klik continue. 
29.	Jika ada tampilan seperti ini lewatkan saja dan klik done. 
30.	Maka install sudah dimulai dan mungkin memakan cukup waktu yang lama. 
31.	Jika sudah di install maka akan muncul tampilan seperti ini lalu klik reboot now.
32.	Isi username serta password yang sudah dibuat tadi 
33.	Dan Ubuntu siap digunakan. 