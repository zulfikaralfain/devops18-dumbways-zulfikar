# Day 3 Aplication In Server
## Deploy Aplikasi wayshub-frontend (NodeJS)
### Instalasi NVM dengan perintaH:
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(108).png?raw=true)
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```
### Eksekusi NVM dan Instalasi NodeJS v14 dan v16 serta gunakan v16 dengan perintah
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(109).png?raw=true)
```
exec bash
```
```
nvm install 16
```
```
nvm use 16
```
### Clone direktori yang telah disediakan dengan perintah
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(110).png?raw=true)
```
git clone https://github.com/dumbwaysdew/wayshub-frontend.git
```
### Masuk direktori wayshub-frontend dan install npm
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(111).png?raw=true)
```
cd wayshub-frontend/
```
```
npm install -y
```
### Menjalankan aplikasi pada Directory wayshub-frontend
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(112).png?raw=true)
```
npm start
```
### 1.6 Membuka aplikasi yang telah berjalan dengan ip address dan port 3000
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(113).png?raw=true)
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(127).png?raw=true)
```
ifconfig
```
```
192.168.2.123:3000
```

# Deploy Golang dengan menampilkan nama masing-masing
### Buat direktori golang dan masuk dengan perintah
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(114).png?raw=true)
```
mkdir golang
```
```
cd golang/
```
### Instalasi GO
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(115).png?raw=true)
```
wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
```
### Menghapus file temporary GO
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(116).png?raw=true)
```
rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit
```
### Memasukan PATH Go
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(116).png?raw=true)
```
sudo nano .bashrc
```
### Masukan script berikut pada line paling terakhir
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(116).png?raw=true)
```
export PATH=$PATH:/usr/local/go/bin
```
### Verifikasi GO yang telah kita install dengan perintah
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(117).png?raw=true)
```
go version
```
### Buat direktori untuk index golang dan masuk dengan perintah
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(120).png?raw=true)
```
mkdir day3go
```
```
cd day33go
```
```
nano index.go
```
### Membuat project index sederhana menggunakan GO
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(119).png?raw=true)
```
package main  
import "fmt"  
func main() {  
    fmt.Println("Zulfikar Alfain Rahman")
}
```
### Menjalankan project index yang telah kita buat dan membuat build agar mudah di jalankan dalam direktori index go yang kita buat
![alt texr](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(120).png?raw=true)
```
go run index.go
```
```
go build index.go
```
```
./index.go
```

# Deploy python dengan menampilkan nama masing-masing
### Membuat direktori python dan verifikasi python karna sudah terinstall pada ubuntu jadi kita install package manager saja
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(121).png?raw=true)
```
mkdir python
```
```
cd /python
```
```
python3 -V
```
```
sudo apt-get install python3-pip
```
### Instalasi library machine Python dan membuat index sederhana dengan Python
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(122).png?raw=true)
```
pip install flask
```
```
nano index.py
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(123).png?raw=true)
```
from flask import Flask
app = Flask(__name__)
@app.route("/")
def helloworld():
    return "Zulfikar Alfain Rahman"
if __name__ == "__main__":
    app.run(host='0.0.0.0,port='5000')
```
### Menjalankan aplikasi Python kemudian jalankan pada browser dengan ip masing2 dan port 5000
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(124).png?raw=true)
```
python3 index.py
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(126).png?raw=true)
```
192.168.2.123:5000
```
![alt text](https://github.com/zulfikaralfain/devops18-dumbways-zulfikar/blob/assets/Screenshot%20(125).png?raw=true)