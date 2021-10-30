# Jarkom-Modul-2-B08-2021

Nama | NRP |
--- | --- | 
Adam Hadi Prasetyo | 05111940000224 |
Vyra Fania Adelina | 05111940000109 |
Tsania Az Zahra | 05111940000032 |

1.	EniesLobby akan dijadikan sebagai DNS Master, Water7 akan dijadikan DNS Slave, dan Skypie akan digunakan sebagai Web Server. Terdapat 2 Client yaitu Loguetown, dan Alabasta. Semua node terhubung pada router Foosha, sehingga dapat mengakses internet. 
### KONFIGURASI NODES DAN PING-TEST : semua node tersambung dengan internet dan memiliki konfigurasinya masing-masing. Setiap Client disetting nameservernya untuk mengarah pada IP EniesLobby.

EniesLobby : DNS Master

![image](https://user-images.githubusercontent.com/69724694/139506766-cfecf6e4-efe0-4fe8-b6a1-e5145b0b1f45.png)

![image](https://user-images.githubusercontent.com/69724694/139506782-329db486-0326-41c4-80b1-4acacf9fbf0f.png)

![image](https://user-images.githubusercontent.com/69724694/139506806-b48a1d21-e19c-4b43-81a0-7cc428c3e6ae.png)

Water7 : DNS Slave

![image](https://user-images.githubusercontent.com/69724694/139506846-0a4292da-f903-4df9-a7b2-8875af009ffa.png)

![image](https://user-images.githubusercontent.com/69724694/139506852-b78981f5-2aa4-4ed5-96cf-7d6e3ebfa362.png)

Skypie : Webserver

![image](https://user-images.githubusercontent.com/69724694/139506866-a5201157-7b20-4206-9507-695b6228d8b4.png)

![image](https://user-images.githubusercontent.com/69724694/139506876-17d6ffee-71c0-46db-a100-7a959708e13d.png)

Loguetown X Alabasta : Client

![image](https://user-images.githubusercontent.com/69724694/139506884-a2c8b8a7-14b7-4392-b979-955deac054b8.png)

![image](https://user-images.githubusercontent.com/69724694/139506892-c6744a1b-5dfe-490b-8875-d948b692eb35.png)

![image](https://user-images.githubusercontent.com/69724694/139506908-20477de5-1a5f-49f0-ba4d-0174ee23bee2.png)

![image](https://user-images.githubusercontent.com/69724694/139506915-c5353a12-5a89-47da-bf49-c1a42cf6decc.png) 

Foosha : Internet-Source

![image](https://user-images.githubusercontent.com/69724694/139506926-0e5e3a8e-0762-4090-8118-df9bd5e6db8d.png)

![image](https://user-images.githubusercontent.com/69724694/139506929-626df02f-cadf-42d5-a717-799f3d7ae63d.png)

2. Luffy ingin menghubungi Franky yang berada di EniesLobby dengan denden mushi. Kalian diminta Luffy untuk membuat website utama dengan mengakses franky.yyy.com dengan alias www.franky.yyy.com pada folder kaizoku.

### Mendefinisikan franky.b08.com di EniesLobby dan aliasnya menggunakan command dan syntax yang digaris bawah berwarna biru

![image](https://user-images.githubusercontent.com/69724694/139507394-bbdd6d0c-b7e8-40ed-91f8-a9b45f96510f.png)

### Hasil ping melalui client baik dengan atau tanpa alias-name franky.b08.com

![image](https://user-images.githubusercontent.com/69724694/139507134-ddb82cd9-d19e-4156-97a3-78ce4ef687d4.png)

3.  Setelah itu buat subdomain super.franky.yyy.com dengan alias www.super.franky.yyy.com yang diatur DNS nya di EniesLobby dan mengarah ke Skypie.

### Mendefinisikan super.franky.b08.com di EniesLobby dan aliasnya menggunakan command dan syntax yang digaris bawah berwarna biru
![](img/no3.jpg)

4. Buat juga reverse domain untuk domain utama.
   
### Tambahkan konfigurasi zone untuk reverse domain pada file named.conf.local

![](img/no4.jpg)

### Lakukan PTR ke reverse domain yang telah dibuat

![](img/no4%20(2).jpg)

5. 