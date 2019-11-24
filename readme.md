# Pembuatan Topologi

![topologi](https://user-images.githubusercontent.com/42793740/69493243-01dd5600-0edf-11ea-8513-377f9fe3d1e2.PNG)

# Setting IP di tiap UML (nano /etc/network/interfaces)

![ip venusaur](https://user-images.githubusercontent.com/42793740/69493523-41597180-0ee2-11ea-8a38-3826825fb33f.PNG)

![ip arceus](https://user-images.githubusercontent.com/42793740/69493524-41597180-0ee2-11ea-990b-eeb39703102d.PNG)

![ip articuno](https://user-images.githubusercontent.com/42793740/69493525-41f20800-0ee2-11ea-95fe-6258fb23629c.PNG)

![ip blastoise](https://user-images.githubusercontent.com/42793740/69493526-41f20800-0ee2-11ea-92f1-a6538cba0a26.PNG)

![ip mew](https://user-images.githubusercontent.com/42793740/69493527-428a9e80-0ee2-11ea-9d10-0facc072f150.PNG)

![ip mewtwo](https://user-images.githubusercontent.com/42793740/69493528-428a9e80-0ee2-11ea-91fe-f2d1796d0c33.PNG)

![ip moltres](https://user-images.githubusercontent.com/42793740/69493529-428a9e80-0ee2-11ea-8207-fb2cc9813ecc.PNG)

![ip pikachu](https://user-images.githubusercontent.com/42793740/69493530-43233500-0ee2-11ea-909c-109a33def53e.PNG)

![ip psyduck](https://user-images.githubusercontent.com/42793740/69493532-43bbcb80-0ee2-11ea-8cd1-67feaf5e8abf.PNG)

![ip snorlax](https://user-images.githubusercontent.com/42793740/69493533-43bbcb80-0ee2-11ea-969e-8a5f0d24c427.PNG)

# Export Proxy

![proxy](https://user-images.githubusercontent.com/42793740/69493648-b4171c80-0ee3-11ea-84a7-5ae0c5fd4cf8.PNG)

# Routing

![routing arceus](https://user-images.githubusercontent.com/42793740/69493372-ccd20300-0ee0-11ea-964b-115a687dfa95.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.9
```

![routing blastoise](https://user-images.githubusercontent.com/42793740/69493373-cd6a9980-0ee0-11ea-9577-43e2c423ebfe.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.1
```

![routing pikachu](https://user-images.githubusercontent.com/42793740/69493374-cd6a9980-0ee0-11ea-8f6b-e7dc68cb6ee0.PNG)

```
route add -net 192.168.0.128 netmask 255.255.255.128 gw 192.168.0.2
route add -net 10.151.73.16 netmask 255.255.255.248 gw 192.168.0.2
route add -net 192.168.0.8 netmask 255.255.255.252 gw 192.168.0.6
route add -net 192.168.1.0 netmask 255.255.255.0 gw 192.168.0.6
route add -net 192.168.0.16 netmask 255.255.255.248 gw 192.168.0.6 
```

![routing venusaur](https://user-images.githubusercontent.com/42793740/69493375-cd6a9980-0ee0-11ea-92b3-649b9d8cc20d.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.5
route add -net 192.168.0.16 netmask 255.255.255.248 gw 192.168.0.10 
```
# Soal

1. Agar topologi yang kalian buat dapat mengakses keluar, kalian diminta untuk mengkonfigurasi
PIKACHU menggunakan iptables, namun Satoshi melarang kalian menggunakan MASQUERADE
karena terlalu mudah.

Karena keberadaan jaringan tersebut sudah mulai diketahui dari oleh jaringan luar, Satoshi pun
merasa panik, karena merasa jaringannya masih belum aman. 

2. Oleh karena itu maka kalian diminta
untuk mendrop semua akses SSH dari luar Topologi (UML) Kalian pada server yang memiliki ip
DMZ (DHCP dan DNS SERVER) pada PIKACHU demi menjaga keamanan.

3. Karena tim kalian maksimal terdiri dari 2 atau 3 orang saja, Satoshi meminta kalian untuk hanya
membatasi DHCP dan DNS server hanya boleh menerima maksimal 2 atau 3(jumlah kelompok)
koneksi ICMP secara bersamaan yang berasal dari mana saja menggunakan iptables pada masing
masing server, selebihnya akan di DROP.

4. Kalian juga diminta untuk mengkonfigurasi PIKACHU untuk dapat membedakan ketika MEW
diakses dari subnet AJK, akan diarahkan pada MEWTWO dengan port 1234. 

5. Sedangkan ketika
diakses dari subnet INFORMATIKA akan diarahkan pada MOLTRES dengan port 1234.
kemudian kalian diminta untuk membatasi akses ke MEW yang berasal dari SUBNET AJK dan
SUBNET INFORMATIKA dengan peraturan sebagai berikut,:

6. Akses dari subnet AJK hanya diperbolehkan pada pukul 08.00 - 17.00 pada hari Senin sampai
Jumat,

7. Akses dari subnet INFORMATIKA hanya diperbolehkan pada pukul 17.00 hingga pukul
09.00 setiap harinya
Selain itu paket akan di REJECT.
Karena kita memiliki 2 buah WEB Server, 

9.Satoshi ingin PIKACHU disetting sehingga setiap
request dari client yang mengakses DNS Server akan didistribusikan secara bergantian pada
MEWTWO port 80 dan MOLTRES port 80.
Karena banyak paket yang di drop oleh tim kalian, 

10. Satoshi ingin agar semua paket didrop oleh
firewall (dalam topologi) tercatat dalam log pada setiap UML yang memiliki aturan drop.

# Kendala yang dialami 

- Keterbatasan waktu
