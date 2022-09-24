# Jarkom-Modul-1-B09-2022

### Anggota Kelompok
| Nama                 | NRP        |
|----------------------|------------|
| Gery Febrian Setyara | 5025201151 |
| Muhammad Yunus       | 5025201171 |
| Hafiz Kurniawan      | 5025201032 |

### 1. Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!
filter dengan `http` kemudian membuka hypertext yang memuat status 200 OK.<br>

![1](https://user-images.githubusercontent.com/99454377/192098448-317b55f5-f685-4894-bb5c-569713b7f60b.png)

Web server yang digunakan "monta.if.its.ac.id" adalah `nginx/1.10.3`

### 2. Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

Export object dengan langkah pilih `file --> export object`<br>

![201](https://user-images.githubusercontent.com/99454377/192098458-dad04981-8314-4b16-a04b-a74d97b66735.png)

Kemudian simpan id Ishaq (194) dan kemudian tambahkan ektensi pada file dengan menambahkan .html <br>

![202](https://user-images.githubusercontent.com/99454377/192098464-e72a2413-c87a-478b-86cb-b82db31ad895.png)

Lalu buka file tersebut dengan browser <br>

![203](https://user-images.githubusercontent.com/99454377/192098469-26cf1a31-5887-489e-af49-95a5390dbcd3.png)
<br>


### 3.Filter Sehingga Wireshark Hanya Menampilkan Paket Yang Menuju Port 80!

Dilakukan Filtering menggunakan dst(Destination) karena yang diminta adalah port menuju 80

![3](https://user-images.githubusercontent.com/92217354/191956090-d1142091-8f27-451e-8b3f-75619601ff2b.jpeg)


### 4.Filter Sehingga Wireshark Hanya Menampilkan Paket Yang Berasal dari Port 21!

Dilakukan Filtering menggunakan src(Source) karena yang diminta adalah port berasal 21

![4](https://user-images.githubusercontent.com/92217354/191956548-8fa27232-fcd8-4d5a-b42d-b1a1480f8151.jpeg)


### 5.Filter Sehingga Wireshark Hanya Menampilkan Paket Yang Berasal dari Port 443!

Dilakukan Filtering menggunakan src(Source) karena yang diminta adalah port berasal 443

![5](https://user-images.githubusercontent.com/92217354/191956772-1c5d84b7-8ff8-4244-866d-6ea8a22c0808.jpeg)


### 6.Filter Sehingga Wireshark Hanya Menampilkan Paket Yang Menuju ke "lipi.go.id"

Dilakukan Filtering menggunakan http karena yang diminta adalah web ke "lipi.go.id"

![6](https://user-images.githubusercontent.com/92217354/191957199-dae18f03-ad09-4993-8ac9-6fd9ebda373d.jpeg)

### 7.Filter Sehingga Wireshark Hanya Menampilkan Paket Yang Berasal dari IP Kalian!

Dilakukan Capture Filtering menggunakan src 192.168.18.1 karena IP tersebut adalah IP Saya

![7](https://user-images.githubusercontent.com/92217354/191957466-a4288761-e102-4230-bdaf-9aa9616bdf3f.jpeg)

### 8. Percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum.
![image](https://user-images.githubusercontent.com/70748569/192000084-cc11a74a-7c71-4a2e-9ab2-c2ea00860483.png)
![image](https://user-images.githubusercontent.com/70748569/192000244-45e66191-d982-4bf4-b169-f00c46f8e4aa.png)
![image](https://user-images.githubusercontent.com/70748569/192000329-ec719564-b690-4b96-a9bf-f1a7f9eca746.png)

Dari percakapan yang ada, diketahui bahwa file berada pada port 9002, sehingga dilakukan filter ``tcp.port == 9002``. dan ditemukan pesan sebagai berikut
![image](https://user-images.githubusercontent.com/70748569/192000390-93fc38c5-dbe9-4dac-8387-b0f7d6ce860e.png)

### 9. File yang ditemukan merupak pesan yang telah di-encrypt yang harus di decrypt menggunakan openssl dengan methode des3. sebagai berikut
![image](https://user-images.githubusercontent.com/70748569/192001255-d5d69947-c063-4985-adea-1368e50bf10a.png)

Selanjutnya file disimpan sebagai `raw` dengan format `des3`, dengan nama file `B09.des3`
![image](https://user-images.githubusercontent.com/70748569/192001600-bebe7542-94f8-4281-aaaf-52a7aa1fea74.png)

setelah disimpan, file di-decrypt menggunakn openssl dengan methode des3. dengan command bash 
```bash 
openssl des3 -salt -in B09.des3 -out flag.txt
```
selanjutnya akan diminta untuk memasukkan password. password untuk file berdasarkan clue yang diberikan dari percakapan adalah nama dari kembar 5 yang merujuk pada suatu anime [go-toubun hayanome](https://myanimelist.net/anime/39783/5-toubun_no_Hanayome_%E2%88%AC), kesamaan diantaran mereka, dan dalam huruf kecil. Oleh karena itu jawabannya adalah *nakano yang merupakan nama keluarga dari kembar 5.
![image](https://user-images.githubusercontent.com/70748569/192002975-26b1c52f-9c3d-405c-959d-e83c5d7deacd.png)

dan didapatkan hasil pada flag.txt sebagai berikut.
![image](https://user-images.githubusercontent.com/70748569/192003240-b489a142-226b-4fa4-b912-9765dd2ccac8.png)

### 10. Flag yang ditemukan adalah 
> JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}
