# Auto Backup
Terms Of Service:
1. By purchasing and using a service from Orume Studios means you have agreed to this Terms of Service.
2. You are not allowed to sell or redistribute.
3. You may only use this script on your own machine not others.
4. You will not share any files or data from this resource, this includes screenshots, lines of code or files.
5. You will not steal any code for your project/script or even private purposes.
6. You must always follow our rules. Breaking any of them will get you banned

Note: you may only use auto-backup on linux distros. (tested on Debian-based linux, RHEL - Cent Os - Rocky - Enterprise linux), using this script with chocolate or ws may works on windows but not tested.



=================================================================================================
For the installation of the package, use according to the distro you are using, if it is ubuntu or debian-like distro then use apt-get, else if you are using an enterprise linux distro then use dnf or yum.

English:
1. Update linux packages:
On debian-based:
apt-get update -y

On enterprise:
dnf update -y
yum update -y

2. Install unzip and zip, run the following commands:
On debian-based:
apt-get install zip unzip

On enterprise:
yum install zip unzip
dnf install zip unzip

3. Create a folder for the autobackup configurations
The default folder is `/etc/auto-backup`, run the following command to create the folder:
mkdir -p /etc/auto-backup

4. Upload the auto backup zip (on anywhere) and decompress the zip:

Run the following command if you have uploaded the zip file:
unzip auto-backup.zip

5. Install the auto backup on a different path, go to the directory where the extracted auto backup is and run the following command:
chmod +x install.sh
bash install.sh

6. If you are prompted "Enter your config path:"
Enter the path where you have created the auto backup configuration folders on step 3, the default one is `/etc/auto-backup`.

7. Install rclone on your PC, go to https://rclone.org/downloads/
I'm using a windows PC, if you are, go for the AMD 64 Bit version (Windows) for it.

6. Configure your rclone, docs reference: https://rclone.org/drive/,
Watch the following video:
the video is still on progress, please open a ticket on our discord for an assistance.

you can skip to step 7 if you understand how to configure rclone.


7. Run the backup script depends on your configuration path, the defauilt one is `/etc/auto-backup`
run the following command to test:
echo "/etc/auto-backup" | bash /usr/bin/backup

8. Setup cronjobs
run the following command: 
crontab -e

if you are using nano:
type "0 0 * * * echo "/etc/auto-backup" | bash /usr/bin/backup
press ctrl + x, press y and enter

if you are using vi:
press s, 
type "0 0 * * * echo "/etc/auto-backup" | bash /usr/bin/backup
press esc, press :wq and enter

9. Configure the configurations as you want:
There is two configurations file.

lang.conf - The language configuration such as webhooks or messages.
config.conf - The main configuration such as the location of the backup folder, cloud, remote clone, and others

Congratulations you're done! if you don't understand how to install, you may order a service installation for $2.0, or a support for free.
=================================================================================================
1. Dengan membeli dan menggunakan layanan dari Orume Studios berarti Anda telah menyetujui Ketentuan Layanan ini.
2. Anda tidak diperbolehkan untuk menjual atau mendistribusikan kembali.
3. Anda hanya dapat menggunakan skrip ini di mesin Anda sendiri, bukan orang lain.
4. Anda tidak akan membagikan file atau data apa pun dari sumber ini, termasuk tangkapan layar, baris kode, atau file.
5. Anda tidak akan mencuri kode apa pun untuk proyek/skrip Anda atau bahkan untuk tujuan pribadi.
6. Anda harus selalu mengikuti aturan kami. Melanggar salah satu dari mereka akan membuat anda menjadi blacklist kami

MOHON JANGAN MENJADI BOCIL TOLOL YANG MENYEBARKAN SCRIPT KARENA TIDAK DI ENCRYPT ATAUPUN DI LISENSI, PAHAMI INI SEBAGAI DEVELOPER HARGAI JANGAN MEMBAJAK.

Untuk installasi packages nya, sesuai dengan distro yang anda gunakan, kalau debian atau seperti ubuntu maka gunakan apt-get, kalau enterprise maka gunakan dnf atau yum.

Indonesia:
1. Update linux packages:
OS debian-based:
apt-get update -y

OS Enterprise:
dnf update -y
yum update -y

2. Install unzip and zip, ketik & enter commands / perintah dibawah:
OS debian-based:
apt-get install zip unzip

OS Enterprise:
yum install zip unzip
dnf install zip unzip

3. Buat folder baru untuk konfigurasi autobackupnya, bawaannya adalah `/etc/auto-backup`

Ketik perintah berikut untuk membuat folder:
mkdir -p /etc/auto-backup

4. Upload auto backup zipnya (bebas dimana) lalu decompress zipnya:
Sesudah kamu upload, ketik dan enter command: `unzip auto-backup.zip`

5. Install auto backupnya di path/tempat yang berbeda, lalu masuk/pergi ke folder yang dimana berisi auto backup yang telah di extract, dan ketik perintah berikut:
chmod +x install.sh
bash install.sh

6. Jika kamu ditanyakan "Enter your config path:"
Masukan pathnya sesuai path yang anda buat di step 3, bawaannya adalah `/etc/auto-backup`.


7. Install rclone di pc kamu, ke website https://rclone.org/downloads/
Saya sih pakai PC windows, jadi kalau kamu juga pakai windows install versi AMD 64 Bit (Windows) untuk itu.

6. Konfigurasi rclone kamu, docs reference: https://rclone.org/drive/,
Tonton video dibawah ini:
belum ada videonya, open tiket di discord ya untuk bantuannya.

Kamu bisa skip ke step 7 jika kamu paham cara mengkonfigurasikan rclone.


7. Jalankan script backupnya sesuai konfigurasi kamu, bawaan dari awalnya pathnya itu `/etc/auto-backup`
ketik dan enter command dibawah untuk menguji atau memulai backupnya.
echo "/etc/auto-backup" | bash /usr/bin/backup

8. Setup cronjobs
ketik dan jalankan command dibawah:
crontab -e

if you are using nano:
type "0 0 * * * echo "/etc/auto-backup" | bash /usr/bin/backup
tekan ctrl + x di keyboard secara bersamaan, ketik y dan enter

if you are using vi:
press s, 
type "0 0 * * * echo "/etc/auto-backup" | bash /usr/bin/backup
tekan esc di keyboard, ketik :wq dan enter

9. Di setup konfigurasinya sesuai dengan yang kamu inginkan:
Ada dua konfigurasi

lang.conf - ini untuk menambahkan webhooks atau pesan
config.conf - ini untuk memodifikasi konfigurasi utama seperti letak folder backup, cloud, remote rclonenya, dan lain-lain

Selamat Anda sudah selesai! jika anda tidak mengerti bagaimana cara menginstal, anda dapat memesan instalasi layanan seharga $2,0, atau open ticket support secara gratis.