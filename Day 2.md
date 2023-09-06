# Day 2 Basic Shell & Computer Networking
## Perbedaan IP Private & Public, Serta Ip Dynamic & Static
**IP Private vs. IP Public**:

**IP Private** adalah alamat IP yang digunakan di dalam jaringan lokal atau LAN (Local Area Network) Anda. IP-private ini tidak dapat diakses langsung dari internet, dan biasanya digunakan untuk mengidentifikasi perangkat dalam jaringan lokal. Beberapa contoh dari rentang IP-private yang umum digunakan adalah:

- 192.168.0.0 hingga 192.168.255.255
- 172.16.0.0 hingga 172.31.255.255
- 10.0.0.0 hingga 10.255.255.255

**IP Public**, di sisi lain, adalah alamat IP yang dapat diakses dari internet. Ini adalah alamat yang digunakan untuk mengidentifikasi perangkat atau server di internet. Setiap perangkat yang terhubung langsung ke internet memiliki alamat IP publik yang unik. IP publik diberikan oleh penyedia layanan internet (ISP) dan digunakan untuk mengirim dan menerima data melalui internet. Jika Anda mengakses situs web atau layanan online, alamat IP publik server tersebut adalah yang Anda lihat.

**IP Dynamic vs. IP Static**:

**IP Dynamic** adalah jenis alamat IP yang diberikan oleh server DHCP (Dynamic Host Configuration Protocol). Ketika perangkat terhubung ke jaringan, server DHCP akan memberikan alamat IP kepada perangkat tersebut secara dinamis. Ini berarti bahwa setiap kali perangkat terhubung ulang ke jaringan, alamat IP yang diberikan dapat berubah. IP dinamis umumnya digunakan di jaringan rumah dan bisnis kecil.

**IP Static**, di sisi lain, adalah alamat IP yang ditetapkan secara manual untuk perangkat atau server. IP statis tidak berubah secara otomatis. Ini digunakan ketika Anda ingin memastikan bahwa perangkat atau server selalu memiliki alamat IP tertentu. IP statis sering digunakan pada server, router, atau perangkat yang perlu diakses dari luar jaringan.

Perbedaan utama antara IP dinamis dan statis adalah bahwa IP dinamis diberikan oleh server DHCP secara otomatis dan dapat berubah, sedangkan IP statis ditetapkan manual dan tetap tidak berubah kecuali diubah secara manual. IP publik, baik dinamis maupun statis, dapat digunakan untuk mengidentifikasi perangkat di internet, sedangkan IP private digunakan di dalam jaringan lokal dan tidak dapat diakses langsung dari internet.

![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/264198848-ba31c932-2bcb-46f2-b98b-8772fd39fcc4.png?raw=true)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/264923399-b21d987e-bb40-4afc-a2f5-2618d3c36eef.png?raw=true)
**Rancangan sebuah jaringan**

rancangan sebuah jaringan dengan spesifikasi
* CIDR Block : 192.168.1.xxx/24
* Subnet : 255.255.255.0
* Gateway : 192.168.1.1
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/snfasfjoerfwefnooNSOQUWFHQEN.png?raw=true)
**Untuk Diagramnya adalah sebagai berikut**
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Diagram%20Jaringan.png?raw=True)