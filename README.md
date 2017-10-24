# Pendahuluan
# Dasar Teori (Penjelasan OS dan Semua Tools yang digunakan)
# Uji Penetrasi 1
* ## Langkah Instalasi Ubuntu Server
    Kelompok kami menggunakan tools VirtualBox untuk menginstal ubuntu server. Ubuntu server yang kelompok kami gunakan adalah ubuntu server 16.04.3
    
    1. Buka terlebih dahulu virtualbox di PC / Laptop Anda.
    
    ![1](https://user-images.githubusercontent.com/16026826/31867146-3cdc1644-b7b4-11e7-9f25-3fd11c3f17e4.PNG)
    <br>
    2. Isi "name" dengan nama Ubuntu Server. Pada "type" pilih Linux dan pada "version" pilih Ubuntu 64-bit.
    
    ![2](/image1/2.PNG)

    <br>

    3. Pada memory size atur menjadi 2048 MB.
    
    ![3](https://user-images.githubusercontent.com/16026826/31871473-c20a2ab6-b7de-11e7-88d6-d3dbf109fa31.PNG)

    <br>
    4. Hard disk file type pilih menggunakan VDI (VirtualBox Disk Image).

    ![5](https://i.imgur.com/0UQ1Vce.png)
    <br>
    5. Selanjutnya pilih dynamically allocated pada storage on physical hard disk.

    ![6](https://i.imgur.com/SJZLqIe.png)
    <br>
    6. Pada file location ad size, pilih sebesar 10 GB

    ![7](https://i.imgur.com/RkcM9Wo.png)
    <br>
    7. Setelah klik create, maka akan tampil OS baru dengan nama Ubuntu Server. Selanjutnya klik "Settings" disebelah kanan tulisan new.
    
    ![8](https://i.imgur.com/hg9bcEs.png)
    <br>
    8. S Lalu ganti seperti pada gambar di bawah
    
    ![9](https://i.imgur.com/BPBKQbX.png)
    <br>
    9. Pada setting > network, ubah menjadi "bridged adapter" suapaya bisa mendapatkan IP sesuai dengan subnet yang kita gunakan pada PC / laptop yang Anda gunakan.
    
    ![10](https://i.imgur.com/hkmPIGE.png)
    <br>
    10. Pada seting > storage, pilih Optical Drive yang akan Anda gunakan. Disini kelompok kami memilih untuk menggunakan Ubuntu Server 16.04.3.
    
    ![11](https://i.imgur.com/6t4rcCf.png)
    <br>
    11. Anda akan diharuskan memilih seperti pada gambar dibawah. Pilih OS yang akan Anda gunakan. Jika selesai, pada Anda hanya perlu mengklik sampai finish.
    
    ![12](https://i.imgur.com/DnMIljP.png)
    <br>
    12. Setelah virtualbox dijalankan, maka klik Start pada tampilan awal virtualbox. Disini Anda diharuskan memilih bahasa yang akan Anda gunakan, contohnya saja "English"
    
    ![14](https://i.imgur.com/dOSXJBH.png)
    <br>
    13. Setelah itu akan muncul seperti gambar di bawah. Pilih Install Ubuntu Server
    
    ![15](https://i.imgur.com/3RsMRpo.png)
    <br>
    14. Setelah itu Anda diharuskan memilih bahasa terlebih dahulu.
    
    ![16](https://i.imgur.com/KfvzJUA.png)
    <br>

    15. Pada location pilih other karena tidak ada Asia.

    ![17](/image1/17.PNG)
    <br>

    16. Lalu selanjutnya pilih Asia

    ![18](/image1/18.PNG)
    <br>

    17. Lalu selanjutnya pilih Indonesia

    ![19](/image1/19.PNG)
    <br>

    18. Lalu selanjutnya pilih United States.

    ![20](/image1/20.PNG)
    <br>

    19. Pada pilihan detect keboard layout, pilih No supaya proses instalasi bisa berjalan lebih cepat.

    ![21](/image1/21.PNG)
    <br>

    20. Tampilan keyboard yang akan kita gunakan adalah English (US)

    ![22](/image1/22.PNG)
    <br>

    21. Pada pilihan keyboard layout, pilih English (US)

    ![23](/image1/23.PNG)
    <br>

    22. Selanjutnya masukkan nama user untuk ubuntu server Anda. Disini kelompok kami menggunakan "target2" sebagai username dari ubuntu server ini.

    ![24](/image1/24.PNG)
    <br>

    23. Pada pilihan uesrname for your account, masukkan "target2" lagi.

    ![25](/image1/25.PNG)
    <br>

    24. Masukkan password untuk user yang baru saja Anda buat.

    ![26](/image1/26.PNG)
    <br>

    25. Masukkan kembali password yang baru saja Anda ketik untuk verifikasi.

    ![27](/image1/27.PNG)
    <br>

    26. Pada pilihan encrypt your home direcotry, pilih No.

    ![28](/image1/28.PNG)
    <br>

    27. Tunggu hingga prosesnya selesai. Setelah itu pilih "Western (Sumatra, Jakarta, Java, West and Central Kalimantan)" untuk pengaturan waktu.

    ![30](/image1/30.PNG)
    <br>

    28. Pada pilihan partition disk, pilih method manual.

    ![31](/image1/31.PNG)
    <br>

    29. Lalu akan muncul seperti gambar dibawah. Tekan enter pada harddisk yang Anda gunakan.

    ![32](/image1/32.PNG)
    <br>

    30. Tekan yes pada pilihan create new empty partition table on this device.

    ![33](/image1/33.PNG)
    <br>

    31. Tekan enter pada pilihan free space yang tersedia.

    ![34](/image1/34.PNG)
    <br>

    32. Selanjutnya pilih create a new partition.

    ![35](/image1/35.PNG)
    <br>

    33. Pada partition size, pilih sebesar 8.7 GB.

    ![36](/image1/36.PNG)
    <br>

    34. Pilih primary pada partisi yang baru saja Anda buat.

    ![37](/image1/37.PNG)
    <br>

    35. Pilih "beginning" untuk lokasi partisi yang baru saja Anda buat.

    ![38](/image1/38.PNG)
    <br>

    36. Ubah pengaturan parisi seperti pada gambar dibawah, dan juga set Mount Point sebagai / (root).

    ![39](/image1/39.PNG)
    <br>

    37. Partisi sebesar 8.7 GB untuk / (root) sudah selesai Anda buat. Selanjutnya pilih free space yang tersisa.

    ![40](/image1/40.PNG)
    <br>

    38. Selanjutnya pilih create a new partition

    ![41](/image1/41.PNG)
    <br>

    39. Pada pilihan partition size, ketikkan sebanyak 2.0 GB, lalu tekan continue.

    ![42](/image1/42.PNG)
    <br>

    40. Pilih "logical" untuk partisi yang baru saja Anda buat.

    ![43](/image1/43.PNG)
    <br>

    41. Tekan enter pada pilihan "Use As"

    ![44](/image1/44.PNG)
    <br>

    42. Lalu pilih "swap area"

    ![45](/image1/45.PNG)
    <br>

    43. Setelah selesai mengganti menjadi swap area, pilih "Done setting up the partition"

    ![46](/image1/46.PNG)
    <br>

    44. Setelah selesai membuat partisi untuk "root" dan juga "swap area", pilih finish partitioning

    ![47](/image1/47.PNG)
    <br>

    45. Lalu pilih yes pada pilihan write the changes to disks.

    ![48](/image1/48.PNG)
    <br>

    46. Setelah itu terdapat pilihan untuk HTTP Proxy, kosongkan saja jika tidak dibutuhkan.

    ![49](/image1/49.png)
    <br>

    47. Lalu Anda pilih software yang akan diinstal ke ubuntu server Anda. Kelompok kami hanya memilih untuk menginstal standard system utilities dan openssh server.

    ![50](/image1/50.png)
    <br>

    48. Lalu pada pilihan install GRUB boot loader, pilih yes.

    ![51](/image1/51.png)
    <br>

    49. Setelah selesai, maka sistem akan restart dan akan muncul halaman login seperti pada gambar dibawah.

    ![52](/image1/52.png)
    <br>

    50. Setelah itu set IP untuk ubuntu server yang telah Anda buat. Disini kelompok kami menggunakan IP 10.151.36.207.

    ![53](/image1/53.png)
    <br>
    
    51. Lalu cek IP pada ubuntu server yang telah Anda buat dengan mengetikkan ifconfig.

    ![54](/image1/54.png)
    <br>



* ## Langkah Instalasi SSH Server
* ## Langkah Uji Penetrasi dengan SSH Brute Force Tools
Tools yang kami gunakan untuk SSH brute force tools antara lain:
1. Hydra
Pada OS Kali Linux 2017 sudah terinstal Hydra, jadi kelompok kami tidak perlu untuk mendownloadnya terlebih dahulu.
    * Langkah pertama Anda harus membuat sebuah file yang memuat beberapa password yang akan dicoba. Kelompok kami membuat file bernama "password.txt".
    * Ketikkan <b>hydra -l target2 -P 'password.txt' 10.151.36.207 ssh</b>. Setelah itu maka akan dilakukan brute force ke target tersebut.

    ![54](/image3/1.png)
    <br>

2. Ncrack
Pada OS kali Linux