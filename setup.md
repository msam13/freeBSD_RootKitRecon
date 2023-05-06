# Setting up freeBSD 12.4 in vmware workstation

ISO - https://download.freebsd.org/releases/amd64/amd64/ISO-IMAGES/12.4/FreeBSD-12.4-RELEASE-amd64-disc1.iso <br>
Video : https://www.youtube.com/watch?v=58GtVfOR_js

## Steps to install SUDO 
<i> login as root </i> <br>

Install pkg tool for install sudo <br>
> root$ /usr/sbin/pkg -v <br>
> root$ pkg update <br>

install sudo <br>
> pkg install sudo <br>

Add desired user to wheel and reboot
> mount -u -w / <br>
> pw usermod "username" -G wheel <br>
> reboot <br>

## Download corresponding header file for 12.4
<i> SSH to freebsd <i>

> fetch ftp://ftp.freebsd.org/pub/FreeBSD/releases/arm64/12.4-RELEASE/src.txz <br>
> tar -C / -xzvf src.txz <br>
> reboot <br>

