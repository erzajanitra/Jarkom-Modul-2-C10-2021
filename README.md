# Jarkom-Modul-2-C10-2021

## Anggota Kelompok C10
| Nama | NRP |
| ------------- | ------------- |
| Christian Bennett Robin | 05111940000078  |
| Erza Janitradevi Nadine  | 05111940000153  |
| Akmal Zaki Asmara  | 05111940000154  |

## Soal dan Pembahasan
### No 1
- Membuat topologi yang terdiri dari EniesLobby sebagai DNS Master, Water7 sebagai DNS Slave, Skypie sebagai webserver, dan Alabasta serta Loguetown sebagai client yang terhubung dengan Foosha. Berikut adalah gambar topologi yang telah dibuat : <br/>
![topologi](https://user-images.githubusercontent.com/75319371/139427788-8f44ed4a-f0cc-4f89-ac60-8a0e532568de.JPG)
- Masing-masing node dapat mengakses internet, hal ini ditunjukkan dengan melakukan ping ke google.com
     - Loguetown
      ![image](https://user-images.githubusercontent.com/75319371/139429185-3422f11e-ea5c-41ba-b2e9-12ea28a02d0d.png)
     - Alabasta
      ![image](https://user-images.githubusercontent.com/75319371/139429651-a01d9ec9-c732-48c4-9e36-e34c1bacf238.png)
     - EniesLobby
      ![image](https://user-images.githubusercontent.com/75319371/139429738-04aa89f0-45bb-4ecc-8e8a-cb1d0cecb6e1.png)
     - Water7
       ![image](https://user-images.githubusercontent.com/75319371/139429406-9939aab0-cc3f-42ba-8296-b33c6eba0203.png)
     - Skypie
      ![image](https://user-images.githubusercontent.com/75319371/139429358-725b93b1-0f94-4cf9-a8c4-a28af2169e60.png)

### No 2
- Membuat website utama dengan mengakses franky.yyy.com dengan alias www.franky.yyy.com pada folder kaizoku 
- Menambahkan zone franky.c10.com pada file `/etc/bind/named.conf.local`
  ```
  zone "franky.c10.com" {
    type master;
    file "/etc/bind/kaizoku/franky.c10.com";
  };
  ```
- Membuat folder kaizoku pada `/etc/bind/` dengan command`mkdir /etc/bind/kaizoku`, kemudian membuat file config `franky.c10.com`
- Memodifikasi config pada file `/etc/bind/kaizoku/franky.c10.com`. Menggunakan NS untuk mendelegasikan zone yang telah dibuat pada franky.c10.com, kemudian domain dipetakan pada IP Enieslobby yaitu `10.19.2.2`. Untuk membuat alias www.franky.c10.com menggunakan CNAME. Berikut adalah modifikasi config yang telah dilakukan:
![config1 - Copy](https://user-images.githubusercontent.com/75319371/139430839-52828f87-3d9a-4e51-8b22-a2318c1ad0e9.JPG)

### No 3
### No 4
### No 5
### No 6
### No 7
### No 8
### No 9
### No 10
### No 11
### No 12
### No 13
### No 14
### No 15
### No 16
### No 17
