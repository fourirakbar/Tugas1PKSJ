# Pendahuluan

**Anggota Kelompok**
1. Aviananda Dwirahma - 5114100085
2. Fourir AKbar - 5114100115
3. Afif Ridho Kamal Putra - 5114100173

# Dasar Teori 
**1. OS yang digunakan**
##### * Ubuntu Server
Ubuntu server adalah sebuah sistem operasi linux berbasis debian yang digunakan untuk membangun sebuah server.

##### * Kali Linux
Kali Linux adalah sebuah distro linux yang merupakan sebuah OS pembaharuan dari BackTRack dan dikembangkan oleh Offensive Security yang mempunyai fungsi untuk kebutuhan professional penetration tester. 

**2. Tools yang digunakan**
##### * Hydra
Hydra adalah sebuah <i>tools</i> untuk membobol <i>remote authentication service</i> dengan metode <i>brute-force attack</i> Hydra dapat melakukan serangan dengan menggunakan <i>dictionary</i> (kamus) terhadap lebuh dari 50 protokol termasuk telnet, ftp, http, https, smb, beberapa databases, and masih banyak lagi. 
##### * Ncrack
Ncrack adalah sebuah <i>tools</i> untuk membobol autentikasi di jaringan dengan kecepatan tinggi. Ncrack dibuat untuk membantu perusahaan mengamankan jaringan mereka dengan proaktif mencoba semua <i>host</i> dan perangkat jaringan yang memiliki <i>password</i> yang lemah. Ahli keamanan (bidang IT) juga mengandalkan ncrack saat meng-audit klien mereka.
##### * Fail2ban
Fail2Ban adalah sebuah layanan yang membuat aturan yang otomatis mengubah iptables pada configurasi firewall berdasarkan percobaan dari banyaknya login yang gagal. dan ini akan mempersilahkan server tersebut (yang dipasang fail2ban) untuk mengharamkan percobaan akses tanpa intervensi dari pemilik server.

# Uji Penetrasi 1
### Tugas:
* Instal sebuah virtual OS dengan Ubuntu Server
* Install SSH server dengan konfigurasi default
* Instal satu lagi virtual OS dengan OS bebas
* Pastikan tools untuk SSH brute force attak sudah terinstall
* Lakukan uji penetrasi 1 dengan THC-Hydra atau Ncrack 

* ## Langkah Instalasi Ubuntu Server
    Kelompok kami menggunakan tools VirtualBox untuk menginstal ubuntu server. Ubuntu server yang kelompok kami gunakan adalah ubuntu server 16.04.3
    
    * Buka terlebih dahulu virtualbox di PC / Laptop Anda.
    
    ![1](https://user-images.githubusercontent.com/16026826/31867146-3cdc1644-b7b4-11e7-9f25-3fd11c3f17e4.PNG)
    <br>
    * Isi "name" dengan nama Ubuntu Server. Pada "type" pilih Linux dan pada "version" pilih Ubuntu 64-bit.
    
    ![2](/image1/2.PNG)

    <br>

    * Pada memory size atur menjadi 2048 MB.
    
    ![3](https://user-images.githubusercontent.com/16026826/31871473-c20a2ab6-b7de-11e7-88d6-d3dbf109fa31.PNG)

    <br>
    * Hard disk file type pilih menggunakan VDI (VirtualBox Disk Image).

    ![5](https://i.imgur.com/0UQ1Vce.png)
    <br>
    * Selanjutnya pilih dynamically allocated pada storage on physical hard disk.

    ![6](https://i.imgur.com/SJZLqIe.png)
    <br>
    *Pada file location ad size, pilih sebesar 10 GB

    ![7](https://i.imgur.com/RkcM9Wo.png)
    <br>
    *Setelah klik create, maka akan tampil OS baru dengan nama Ubuntu Server. Selanjutnya klik "Settings" disebelah kanan tulisan new.
    
    ![8](https://i.imgur.com/hg9bcEs.png)
    <br>
    * S Lalu ganti seperti pada gambar di bawah
    
    ![9](https://i.imgur.com/BPBKQbX.png)
    <br>
    * Pada setting > network, ubah menjadi "bridged adapter" suapaya bisa mendapatkan IP sesuai dengan subnet yang kita gunakan pada PC / laptop yang Anda gunakan.
    
    ![10](https://i.imgur.com/hkmPIGE.png)
    <br>
    * Pada seting > storage, pilih Optical Drive yang akan Anda gunakan. Disini kelompok kami memilih untuk menggunakan Ubuntu Server 16.04.3.
    
    ![11](https://i.imgur.com/6t4rcCf.png)
    <br>
    * Anda akan diharuskan memilih seperti pada gambar dibawah. Pilih OS yang akan Anda gunakan. Jika selesai, pada Anda hanya perlu mengklik sampai finish.
    
    ![12](https://i.imgur.com/DnMIljP.png)
    <br>
    * Setelah virtualbox dijalankan, maka klik Start pada tampilan awal virtualbox. Disini Anda diharuskan memilih bahasa yang akan Anda gunakan, contohnya saja "English"
    
    ![14](https://i.imgur.com/dOSXJBH.png)
    <br>
    * Setelah itu akan muncul seperti gambar di bawah. Pilih Install Ubuntu Server
    
    ![15](https://i.imgur.com/3RsMRpo.png)
    <br>
    * Setelah itu Anda diharuskan memilih bahasa terlebih dahulu.
    
    ![16](https://i.imgur.com/KfvzJUA.png)
    <br>

    * Pada location pilih other karena tidak ada Asia.

    ![17](/image1/17.PNG)
    <br>

    * Lalu selanjutnya pilih Asia

    ![18](/image1/18.PNG)
    <br>

    * Lalu selanjutnya pilih Indonesia

    ![19](/image1/19.PNG)
    <br>

    * Lalu selanjutnya pilih United States.

    ![20](/image1/20.PNG)
    <br>

    * Pada pilihan detect keboard layout, pilih No supaya proses instalasi bisa berjalan lebih cepat.

    ![21](/image1/21.PNG)
    <br>

    * Tampilan keyboard yang akan kita gunakan adalah English (US)

    ![22](/image1/22.PNG)
    <br>

    * Pada pilihan keyboard layout, pilih English (US)

    ![23](/image1/23.PNG)
    <br>

    * Selanjutnya masukkan nama user untuk ubuntu server Anda. Disini kelompok kami menggunakan "target2" sebagai username dari ubuntu server ini.

    ![24](/image1/24.PNG)
    <br>

    * Pada pilihan uesrname for your account, masukkan "target2" lagi.

    ![25](/image1/25.PNG)
    <br>

    * Masukkan password untuk user yang baru saja Anda buat.

    ![26](/image1/26.PNG)
    <br>

    * Masukkan kembali password yang baru saja Anda ketik untuk verifikasi.

    ![27](/image1/27.PNG)
    <br>

    * Pada pilihan encrypt your home direcotry, pilih No.

    ![28](/image1/28.PNG)
    <br>

    * Tunggu hingga prosesnya selesai. Setelah itu pilih "Western (Sumatra, Jakarta, Java, West and Central Kalimantan)" untuk pengaturan waktu.

    ![30](/image1/30.PNG)
    <br>

    * Pada pilihan partition disk, pilih method manual.

    ![31](/image1/31.PNG)
    <br>

    * Lalu akan muncul seperti gambar dibawah. Tekan enter pada harddisk yang Anda gunakan.

    ![32](/image1/32.PNG)
    <br>

    * Tekan yes pada pilihan create new empty partition table on this device.

    ![33](/image1/33.PNG)
    <br>

    * Tekan enter pada pilihan free space yang tersedia.

    ![34](/image1/34.PNG)
    <br>

    * Selanjutnya pilih create a new partition.

    ![35](/image1/35.PNG)
    <br>

    * Pada partition size, pilih sebesar 8.7 GB.

    ![36](/image1/36.PNG)
    <br>

    * Pilih primary pada partisi yang baru saja Anda buat.

    ![37](/image1/37.PNG)
    <br>

    * Pilih "beginning" untuk lokasi partisi yang baru saja Anda buat.

    ![38](/image1/38.PNG)
    <br>

    * Ubah pengaturan parisi seperti pada gambar dibawah, dan juga set Mount Point sebagai / (root).

    ![39](/image1/39.PNG)
    <br>

    * Partisi sebesar 8.7 GB untuk / (root) sudah selesai Anda buat. Selanjutnya pilih free space yang tersisa.

    ![40](/image1/40.PNG)
    <br>

    * Selanjutnya pilih create a new partition

    ![41](/image1/41.PNG)
    <br>

    * Pada pilihan partition size, ketikkan sebanyak 2.0 GB, lalu tekan continue.

    ![42](/image1/42.PNG)
    <br>

    * Pilih "logical" untuk partisi yang baru saja Anda buat.

    ![43](/image1/43.PNG)
    <br>

    * Tekan enter pada pilihan "Use As"

    ![44](/image1/44.PNG)
    <br>

    * Lalu pilih "swap area"

    ![45](/image1/45.PNG)
    <br>

    * Setelah selesai mengganti menjadi swap area, pilih "Done setting up the partition"

    ![46](/image1/46.PNG)
    <br>

    * Setelah selesai membuat partisi untuk "root" dan juga "swap area", pilih finish partitioning

    ![47](/image1/47.PNG)
    <br>

    * Lalu pilih yes pada pilihan write the changes to disks.

    ![48](/image1/48.PNG)
    <br>

    * Setelah itu terdapat pilihan untuk HTTP Proxy, kosongkan saja jika tidak dibutuhkan.

    ![49](/image1/49.png)
    <br>

    * Lalu Anda pilih software yang akan diinstal ke ubuntu server Anda. Kelompok kami hanya memilih untuk menginstal standard system utilities dan openssh server.

    ![50](/image1/50.png)
    <br>

    * Lalu pada pilihan install GRUB boot loader, pilih yes.

    ![51](/image1/51.png)
    <br>

    * Setelah selesai, maka sistem akan restart dan akan muncul halaman login seperti pada gambar dibawah.

    ![52](/image1/52.png)
    <br>

    * Setelah itu set IP untuk ubuntu server yang telah Anda buat. Disini kelompok kami menggunakan IP 10.151.36.207.

    ![53](/image1/53.png)
    <br>
    
    * Lalu cek IP pada ubuntu server yang telah Anda buat dengan mengetikkan ifconfig.

    ![54](/image1/54.png)
    <br>


* ## Langkah instalasi OS Untuk Penetrasi
    OS untuk penetrasi yang kelompok kami gunakan adalah Kali Linux 2017. Kelompok kami menginstal kali linux menggunakan tools virtualbox.

    * Buka terlebih dahulu virtualbox pada PC / laptop Anda, lalu buat virtual machine baru dengan mengklik tombol "new"

    ![1](/image2/1.PNG)
    <br>

    * Lalu atur memory size menjadi 1024 MB

    ![2](/image2/2.PNG)
    <br>

    * Lalu pilih "create a virtual hard disk now"

    ![3](/image2/3.PNG)
    <br>

    * Pada hard disk file type, pilih VDI (VirtualBox Disk Image)

    ![4](/image2/4.PNG)
    <br>

    * Lalu pilih "dynamically allocated" pada pilihan storage on physical hard disk.

    ![5](/image2/5.PNG)
    <br>

    * Untuk size dari hard disknya, pilih 20 GB.

    ![6](/image2/6.PNG)
    <br>

    * Lalu buka seting > storage. Pada optical drive, klik gambar CD untuk memilih image yang akan Anda install.

    ![7](/image2/7.PNG)
    <br>

    * Setelah Anda pilih image yang akan Anda gunakan, disini kelompok kami menggunakan Kali Linux Light 2017, klik OK

    ![8](/image2/8.PNG)
    <br>

    * Lalu masuk ke pilihan network, ganti adapter 1 > attached to menjadi "bridged adapter" supaya virtual machine yang Anda buat bisa mendapatkan IP sesuai subnet PC / laptop Anda.

    ![9](/image2/9.PNG)
    <br>

    * Setelah semua settingan selesai, jalankan virtual machine yang baru saja Anda buat. Setelah itu pilih "install".

    ![10](/image2/10.png)
    <br>

    * Pada pilihan bahasa, pilih English.

    ![11](/image2/11.png)
    <br>

    * Lalu pilih "other" pada territory or area.

    ![12](/image2/12.png)
    <br>

    * Pilih Asia pada pilihan continet or region

    ![13](/image2/13.png)
    <br>

    * Setelah itu pilih Indonesia

    ![14](/image2/14.png)
    <br>

    * Setelah itu pilih United States untuk layout dari keyboard yang akan Anda gunakan.

    ![15](/image2/15.png)
    <br>

    * Pilih American English pada pilihan keymap to use.

    ![16](/image2/16.png)
    <br>

    * Lalu akan ada kolom untuk mengisi hostname. Kelompok kami menggunakan nama "kali" sebagai hostname.

    ![17](/image2/17.png)
    <br>

    * Setelah itu akan ada pilihan domain name. Tidak usah di isi jika tidak perlu.

    ![18](/image2/18.png)
    <br>

    * Setelah itu Anda diharuskan mengisi root password. Jika sudah, enter di continue.

    ![19](/image2/19.png)
    <br>

    * Lalu masukkan kembali root password untuk verifikasi ulang.

    ![20](/image2/20.png)
    <br>

    * Pilih western (Sumatra, Jakarta, Java, Wes and Central Kalimantan) untuk pengaturan waktu.

    ![21](/image2/21.png)
    <br>

    * Pada pilihan partitioning, pilih "guided - use entire disk" supaya proses partisi lebih cepat.

    ![22](/image2/22.png)
    <br>

    * Setelah itu pilih virtual hard disk yang anda gunakan.

    ![23](/image2/23.png)
    <br>

    * Lalu pada pilihan partitioning scheme, pilih "all files in one partition".

    ![24](/image2/24.png)
    <br>

    * Maka secara otomatis akan dibuatkan partisi untuk root (/) dan juga untuk swap area. Setelah itu pilih finish partitioning.

    ![25](/image2/25.png)
    <br>

    * Akan muncul tampilan konfirmasi, tekan yes jika Anda sudah merasa partisi yang Anda lakukan adalah benar.

    ![26](/image2/26.png)
    <br>

    * Lalu pilih yes pada pilihan use a network mirror.

    ![27](/image2/27.png)
    <br>

    * Setelah itu pilih yes pada pilihan install grub boot loader

    ![28](/image2/28.png)
    <br>

    * Pilih tempat untuk menginstal boot loadernya, pilih virtual hard disk yang Anda gunakan.

    ![29](/image2/29.png)
    <br>

    * Setelah itu tunggu proses instalasi berjalan. Jika sudah selesai, maka pilih continue dan sistem akan melakukan restart virtual machine Anda.

    ![30](/image2/30.png)
    <br>

* ## Langkah Instalasi SSH Server
Kelompok kami menginstal SSH server langsung pada saat menginstal ubuntu server.

![50](/image1/50.png)
    <br>
Pada gambar diatas, sistem akan langsung otomatis menginstal openssh-server


* ## Langkah Uji Penetrasi dengan SSH Brute Force Tools
Tools yang kami gunakan untuk SSH brute force tools antara lain:
1. Hydra
Pada OS Kali Linux 2017 sudah terinstal Hydra, jadi kelompok kami tidak perlu untuk mendownloadnya terlebih dahulu.
    * Langkah pertama Anda harus membuat sebuah file yang memuat beberapa password yang akan dicoba. Kelompok kami membuat file bernama "password.txt".
    * Ketikkan <b>hydra -l target2 -P 'password.txt' 10.151.36.207 ssh</b>. Setelah itu akan dilakukan brute force ke target tersebut.

    ![54](/image3/1.png)
    <br>

    * Dapat dilihat pada gambar sebelumnya, jika didapatkan informasi host: 10.151.36.207 login: target2 dan password: password. Setelah itu kelompok kami coba untuk ssh ke host 10.151.36.207. Hasilnya seperti pada gambar dibawah

    ![54](/image3/2.png)
    <br>

2. Ncrack
Pada OS kali Linux 2017 sudah terinstall Ncrack, jadi kelompok kami tidak perlu untuk mendownloadnya terlebih dahulu.
    * Langkah pertama Anda harus membuat sebuah file yang memuat beberapa password yang akan dicoba. Kelompok kami membuat file bernama "password.txt".
    * Ketikkan <b>ncrack -p 22 --user target2 -P 'password.txt' 10.151.36.207</b>. Setelah itu akan dilakukan brute force ke taret tersebut.

    ![54](/image3/3.png)
    <br>

    * Informasi yang didapatkan dari gambar sebelumnya juga sama dengan apa yang kami dapatkan dari penggunaan tools hydra, yaitu host dengan IP 10.151.36.207 dan loginnya "target2", dan juga passwordnya adalah "password" 

# Uji Penetrasi 2
#### Tugas:
* Instal fail2ban pada Ubuntu server yang telah diinstal SSH 
* Konfigurasikan SSH server agar tidak menggunakan setting default
* Lakukan uji penetrasi 2 dengan tools yang sama seperti uji penetrasi 1

* ### Langkah Instalasi Fail2ban pada Ubuntu Server  
    1.  Lakukan update sebelum menginstal fail2ban dengan cara mengetikkan:  
        ```
        $ sudo apt-get update
        ``` 
    
    2.  Selanjutnya install fail2ban dengan syntax dibawah ini:
        ```
        $ sudo apt-get install fail2ban
        ```

    3. Buka file ```jail.conf``` untuk mengubah konfigurasi sesuai dengan apa yang diinginkan. Pada uji penetrasi 2 ini, kami mengubah konfigurasi pada bagian ini
        ```
        bantime = 600
        findtime = 120
        maxretry = 3
        ``` 
        ![3](/image4/fail2ban2.png)
        Keterangan : Konfigurasi diatas akan membuat penyerang mendapatkan ban selama 600 detik (10 menit) apabila melakukan attack terhadap server sebanyak 3 kali dalam kurun waktu 120 detik.
    <br>

* ### Pengamanan dengan konfigurasi Fail2ban 
    
    1. Buka Kali Linux kemudian ketik command dibawah ini untuk melakukan penyerangan. ```test``` merupakan username. Pada pengujian ini kami mencoba menebak username server dan salah hingga tiga kali.
        ```
        hydra -l test -P password.txt 10.151.36.207 ssh
        ```
    2. IP penyerang akan di ban selama 600 detik sesuai dengan konfigurasi fail2ban
    ![2](/image4/fail2ban3.png)

* ### Konfigurasi SSH untuk login dengan SSH keys dibanding dengan menggunakan password.
    Menggunakan password untuk mengakses SSH server adalah sesuatu yang kurang aman. jika ada salah satu user yang menggunakan password yang lemah untuk masuk, maka server tersebut tidak akan terjamin keamanannya. untuk menghindari hal ini, gunakan autentikasi ssh key tanpa menggunakan password.
    
    ##### Generate SSH keys pada klien
    untuk meng-generate SSH key pada mesin klien, jalankan command berikut:

    ````
    cd ~/.ssh
    ssh-keygen -t rsa
    ````
    Tekan enter pada setiap pertanyaan. setelah itu akan terbentuk dua file baru ```id_rsa.pub``` (public key) dan ```id_rsa``` (private key).

    ##### buat folder SSH pada server
    pada server buat folder ssh di home
    ```
    mkdir -p ~/.ssh/
    ```

    ##### Copy file public key ke server
    ```
    scp -P "ssh-port" ~/.ssh/id_dsa.pub username@serverip-address:~/.ssh
    ```
    
    ##### Update file public key pada server
    ```
    cat ~/.ssh/id_rsa.pub >> ~/.ssh/authorized_keys
    chmod 700 .ssh
    chmod 600 .ssh/authorized_keys
    rm .ssh/id_rsa.pub
    ```

    Sekarang klien dapat login ssh ke server tanpa menggunakan password.

* ### Pengamanan dengan konfigurasi SSH-server

    Pada Ubuntu Server, buka konfigurasi SSH dengan menuliskan command berikut ini pada terminal
        ```
        $ sudo /etc/ssh/sshd_config
        ```
    
    ##### Menghilangkan password authentication
    Pada uji penetrasi ini, kami mengganti ```PasswordAuthentication``` menjadi ```no```. Tujuannya adalah server akan mengganti akses masuk menggunakan SSH Key dan memblokir akses dari komputer lain kecuali apabila IP tersebut sudah disetujui oleh server kita.
    
    ![10](/image4/10.png)

    ##### Mengubah default Port
    pada <i>defaultnya</i>, kebanyakan dari server menggunakan port 22 untuk koneksi SSH.
    ubah default port dari 22 ke port yang masih belum dipakai servicenya misal 8908:
    ```
    Port 8908
    ```
    ##### Gunakan SSH2
    SSH1 (protocol 1) mengandung banyak kerentanan keamanan. menggunakan SSH2 (protocol 2) sangatlah direkomendasikan. untuk lebih jelasnya baca http://www.snailbook.com/faq/ssh-1-vs-2.auto.html
    ```
    Protocol 2
    ```
    ##### Non-aktifkan root login
    kebanyakan serangan menggunakan root untuk login ke server dengan SSH, ubah konfigurasi pada line PermitRootLogin
    ```
    PermitRootLogin
    ```
    untuk lebih lengkapnya tentang mengamankan SSH server silahkan buka: https://devops.profitbricks.com/tutorials/secure-the-ssh-server-on-ubuntu/

    <br>
    
    ##### Lakukan restart dengan cara
        ```
        $ sudo service ssh restart
        ```
    
    ##### Pada Kali Linux, lakukan penyerangan dengan Hydra seperti pada gambar dibawah ini
    ![12](/image4/12.png)
    <br>
    
    ##### Hasilnya akan muncul error dengan pemberitahuan bahwa server tidak support password authentication.
    ![13](/image4/13.png)
    <br>
    



Referensi:
1.http://www.kalilinuxindo.com/2014/04/pengenalan-distro-kali-linux.html
2.https://en.wikipedia.org/wiki/Ubuntu_(operating_system)#Ubuntu_Server
3.http://sectools.org/tool/hydra/
4.https://nmap.org/ncrack/
5.https://www.digitalocean.com/community/tutorials/how-to-protect-ssh-with-fail2ban-on-ubuntu-14-04
