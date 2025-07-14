# network-journey-topology-

-my journey on learning cisco packet tracer-

#1.konfigurasi dhcp dan dns server (easy level)
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
