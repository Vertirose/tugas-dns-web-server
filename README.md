## TechStack
- [Bind9](https://www.isc.org/bind/) for Domain Name System
- [Apache2](https://httpd.apache.org/) for Web Server
- [Git](https://git-scm.com/) for clone this source file to virtual machine

## Clone Repository
Before you prepare the application for the web server, clone this repository for the source application
``` 
git clone https://github.com/Vertirose/tugas-dns-web-server.git techStack/
```

## Install Bind9 and Apache 2
Download bind9 and apache 2 on the virtual machine using the command below
```
apt install -y bind9 bind9utils dnsutils apache2
```

## Enable Configuration file Apache 2
Disable default configuration files by executing the command
```
a2dissite 000-default.conf
systemctl restart apache2.service
```
Enable the apache 2 configuration file by executing this command
```
a2ensite kelas.conf www-kelas.conf jurusan.conf doc-jurusan.conf
systemctl restart apache2.service
```

## Configuration
Due to personal reasons, I am unable to continue with the tutorial at this point. For further details, please refer to the following link. [Tutorial Instalasi DNS dan Web Server](https://youtu.be/HWHb_EtDezU?si=brPBfOk6WYoCV4Hu)

> Credit tutorial video from [@gurainzu](https://www.youtube.com/@gurainzu) on Youtube

**Have fun taking them all on.**
