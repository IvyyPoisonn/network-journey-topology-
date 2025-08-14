# network-journey-topology-

-my journey on learning cisco packet tracer-

#1.konfigurasi dhcp dan dns server 
<img width="620" height="410" alt="Screenshot 2025-07-15 045215" src="https://github.com/user-attachments/assets/0f2d1dd7-ab76-4a7e-8135-d98e4ec71f9b" />

caranya:
>Hubungkan perangkat menggunakan kabel
.sambungkan pc client/user ke switch memakai kabel ethernet
.sambungkan switch ke server juga memakai kabel yang sama (ethernet)

>konfigurasi dhcp server (di komputer server)
.klik server- tab config - pilih dhcp
.isi pengaturan: pool name(bebas dengan nama apa saja), default gateaway(misal 192.168.1.1), dns server (pakai ip server juga bisa), start ip address, subnet mask(255.255.255.0)
.klik add

>aktifkan layanan dhcp (pastikan tombol service ON)

>cek konfigurasi client(pc user) dan uji koneksi
.bisa menggunakan ping atau nslookup


#2.konfigurasi LAN dan MAN
<img width="481" height="402" alt="Screenshot 2025-08-14 094824" src="https://github.com/user-attachments/assets/341cd05d-27cd-4d02-842b-a5651a305c21" />

Caranya:
(membangun jaringan lokal)
>sediakan beberapa end device dan switch
.sambungkan end device(pc) ke switch menggunakan kabel straight
.konfigurasikan ip address dan netmask dari masing-masing end device(pc)
.lalu cek menggunakan ping ip salah satu end device tersebut
(syarat untuk menyambungkan beberapa end device yang berada dalam satu jaringan LAN harus dalam satu kelas IP/alamat jaringan)

>sediakan beberapa end device dan switch yang berbeda (dengan IP yang berbeda dari server jaringan diatas tadi)
.lakukan cara yang sama dengan diatas menggunakan ip address yang berbeda dari cara diatas
(sehingga sekarang tersedia dua jaringan yang berbeda)

 (cara menyambungkan end device yang berada di switch satu dan switch dua)
>sediakan satu router
>hubungkan dari switch jaringan pertama dan switch jaringan kedua ke router
>hidupkan port status di router
>konfigurasikan ip gateway untuk switch pertama dan kedua dengan menyesuaikan dengan masing-masing ip dari switch tersebut
>setelah masing-masing switch terhubung dengan router (sekaranag tinggal menyambungkan masing-masing end device yang berasal dari masing-masing switch yang berbeda)
>merouting statik
>masukan sumber ip network dan ip network address pada router
>tanbahkan pada routing table
>lalu cek dengan ping
