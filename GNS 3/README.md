# GNS 3
GNS3 adalah aplikasi simulator jaringan (Graphic Simulator Network) berbasis GUI yang di rilis pada tahun 2008. Dengan GNS3 kita bisa mensimulasikan perangkat asli baik dengan bantuan emulator ataupun teknologi virtualisasi.

# Panduan Instalasi GNS 3
Pastikan dalam komputer anda sudah terinstall `VirtualBox` atau `VMware`.
* ## File yang diperlukan :
  * ### 1. GNS 3
    - Untuk mendownload file master GNS3 silahkan kunjungi link berikut [Download GNS 3](https://www.gns3.com/software/download)
  - ### 2. FIle Server (VirtualBox / VMware)
    - Untuk mendownload file server GNS3 silahkan kunjungi link berikut [Download File Server](https://www.gns3.com/software/download-vm)

# Persiapan Server
Ekstrak file server yang sudah didownload.

Buka softwere yang akan kalian gunakan sebagai server, disini saya menggunakan `VirtualBox` 
![VirtualBox](img/vb1.png)

Klik menu `file` kemudian pilih `import`

![VirtualBox](img/vb2.png)

Kemudian klik icon kecil di kanan kolom file lalu cari file server yang sudah di ekstrak tadi (ekstensi `.ova`).

![VirtualBox](img/vb3.png)
![VirtualBox](img/vb4.png)

Klik tombol next

![VirtualBox](img/vb5.png)

Kemudian klik import dan tunggu hingga proses selesai

![VirtualBox](img/vb6.png)
![VirtualBox](img/vb7.png)

Setelah selesai klik file -> Host Newtowk Manager

![VirtualBox](img/vb9.png)

Klik `create` dan enable dhcp server

![VirtualBox](img/vb10.png)

Setelah selesai setting Host Network Manager, jalankan server yang sudah di import

![VirtualBox](img/vb8.png)
![gns1](img/gns2.jpeg)


# Instalasi Di OS Windows
  * Klik 2 kali pada file master yang sudah didwonload
  
  ![gns1](img/gns1.jpeg)
  * Klik Next atau Agre saja pada setiap pop up yang muncul
  
  ![gns](img/gns3.jpeg)
  ![gns](img/gns4.jpeg)
  ![gns](img/gns5.jpeg)
  ![gns](img/gns6.jpeg)
  ![gns](img/gns6.jpeg)
  ![gns](img/gns7.jpeg)
  ![gns](img/gns8.jpeg)
  * Untuk penawaran solarwinds klik saja `no`
  
  ![gns](img/gns11.jpeg)
  ![gns](img/gns12.jpeg)

# Setup GNS 3
* Setelah instalasi selesai maka akan muncul pop up untuk memilih server. Disini saya akan menggunakan server virtual machine
  
  ![gns](img/setup1.jpeg)
  ![gns](img/setup2.jpeg)
  ![gns](img/setup3.jpeg)

    Jika ada pesan error silahkan klik saja ok

* Pada pop up selanjutkan pilih Virtual Box
  
  ![gns](img/setup4.jpeg)
  ![gns](img/setup5.jpeg)

* Setup untuk GNS 3 sudah selesai.
  
# Menambahkan Router Mikrotik Di GNS 3
Secara default GNS 3 tidak menyediakan router, untuk itu kita harus menginput router secara manual

Silahkan Download file Router Mikrotik pada link berikut 

[Router Mikrotik](https://mikrotik.com/download)

Scroll kebawah sampai menemukan Cloud Hosted Router

![router](img/router1.png)

Kemudian download dengan cara mengklik icon save pada kolom `Raw disk image`

Ekstrak file tersebut

Kembali Ke GNS 3, pilih menu edit -> preferences kemudian klik new pada kolom `Qemu VMs`

![router](img/router2.jpeg)

Pilih `Run this Qemu VM on the GNS3 VM`

![router](img/router3.jpeg)

Beri nama untuk router yang akan ditambahkan

![router](img/router4.jpeg)

Next

![router](img/router5.jpeg)

Next

![router](img/router6.jpeg)

Pada pop up ini pilih `New Image` kemudian klik browse... untuk mencari file router mikrotik yang sudah diekstrak (file yang berekstensi `.img`)

![router](img/router7.jpeg)
![router](img/router8.jpeg)

Setelah selesai klik edit

![router](img/router9.jpeg)

Pada tab `General Setting` ubah kategori menjadi `Routers`

![router](img/router10.jpeg)

Pada tab `Network` silahkan ubah pada kolom `Adapters` untuk menambahkan port pada router sesuai kebutuhan anda. Disini saya mengubah router saya menjadi 4 port yang tersedia.

![router](img/router11.jpeg)

Setelah selesai silahkan klik ok maka Router Mikrotik akan muncul pada workspace GNS3

![router](img/router12.jpeg)

  
    