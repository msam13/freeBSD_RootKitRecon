# Setting up freeBSD 12.2 in vmware workstation

FreeBSD 12.2 - http://ftp-archive.freebsd.org/pub/FreeBSD-Archive/old-releases/ISO-IMAGES/12.2/FreeBSD-12.2-RELEASE-amd64-disc1.iso <br>
link : https://www.youtube.com/watch?v=58GtVfOR_js

### Steps to install SUDO 

Step 1 : Boot in single user mode <br>
Step 2 : <br>
> mount -u -w / <br>
> pw usermod "username" -G wheel <br>
> reboot <br>

> pkg update && pkg upgrade <br>
> pkg install sudo <br>

### steps to setup FTP server

