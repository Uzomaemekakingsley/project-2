user@DESKTOP-0MRT209 MINGW64 ~/Downloads/project2 (master)
$ ssh -i "project2.pem" ubuntu@ec2-34-224-165-228.compute-1.amazonaws.com
The authenticity of host 'ec2-34-224-165-228.compute-1.amazonaws.com (34.224.165.228)' can't be established.
ED25519 key fingerprint is SHA256:/cAR9jwprB48mPNtkHip3G7+Mga1+11OYN0ZMhqVYc8.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'ec2-34-224-165-228.compute-1.amazonaws.com' (ED25519) to the list of known hosts.
Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.11.0-1022-aws x86_64)

- Documentation: https://help.ubuntu.com
- Management: https://landscape.canonical.com
- Support: https://ubuntu.com/advantage

System information as of Tue Feb 1 22:47:51 UTC 2022

System load: 0.03 Processes: 102
Usage of /: 18.2% of 7.69GB Users logged in: 0
Memory usage: 20% IPv4 address for eth0: 172.31.21.73
Swap usage: 0%

1 update can be applied immediately.
To see these additional updates run: apt list --upgradable

The list of available updates is more than a week old.
To check for new updates run: sudo apt update

The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/\*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

To run a command as administrator (user "root"), use "sudo <command>".
See "man sudo_root" for details.

ubuntu@ip-172-31-21-73:~$ sudo apt update
Hit:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal InRelease
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates InRelease [114 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports InRelease [108 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 Packages [8628 kB]
Get:5 http://security.ubuntu.com/ubuntu focal-security InRelease [114 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe Translation-en [5124 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 c-n-f Metadata [265 kB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse amd64 Packages [144 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse Translation-en [104 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/multiverse amd64 c-n-f Metadata [9136 B]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages [1546 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main Translation-en [299 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 c-n-f Metadata [14.7 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/restricted amd64 Packages [775 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/restricted Translation-en [111 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/restricted amd64 c-n-f Metadata [532 B]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 Packages [896 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe Translation-en [197 kB]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 c-n-f Metadata [20.0 kB]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 Packages [24.8 kB]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse Translation-en [6928 B]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/multiverse amd64 c-n-f Metadata [620 B]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/main amd64 Packages [42.0 kB]
Get:24 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/main Translation-en [10.0 kB]
Get:25 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/main amd64 c-n-f Metadata [864 B]
Get:26 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/restricted amd64 c-n-f Metadata [116 B]
Get:27 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe amd64 Packages [20.8 kB]
Get:28 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe Translation-en [14.3 kB]
Get:29 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/universe amd64 c-n-f Metadata [692 B]
Get:30 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-backports/multiverse amd64 c-n-f Metadata [116 B]
Get:31 http://security.ubuntu.com/ubuntu focal-security/main amd64 Packages [1178 kB]
Get:32 http://security.ubuntu.com/ubuntu focal-security/main Translation-en [210 kB]
Get:33 http://security.ubuntu.com/ubuntu focal-security/main amd64 c-n-f Metadata [9132 B]
Get:34 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 Packages [686 kB]
Get:35 http://security.ubuntu.com/ubuntu focal-security/restricted Translation-en [97.9 kB]
Get:36 http://security.ubuntu.com/ubuntu focal-security/restricted amd64 c-n-f Metadata [536 B]
Get:37 http://security.ubuntu.com/ubuntu focal-security/universe amd64 Packages [677 kB]
Get:38 http://security.ubuntu.com/ubuntu focal-security/universe Translation-en [115 kB]
Get:39 http://security.ubuntu.com/ubuntu focal-security/universe amd64 c-n-f Metadata [13.0 kB]
Get:40 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 Packages [21.8 kB]
Get:41 http://security.ubuntu.com/ubuntu focal-security/multiverse Translation-en [4948 B]
Get:42 http://security.ubuntu.com/ubuntu focal-security/multiverse amd64 c-n-f Metadata [536 B]
Fetched 21.6 MB in 4s (5651 kB/s)
Reading package lists... Done
Building dependency tree
Reading state information... Done
41 packages can be upgraded. Run 'apt list --upgradable' to see them.
ubuntu@ip-172-31-21-73:~$ sudo apt install nginx
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
fontconfig-config fonts-dejavu-core libfontconfig1 libgd3 libjbig0
libjpeg-turbo8 libjpeg8 libnginx-mod-http-image-filter
libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream libtiff5
libwebp6 libxpm4 nginx-common nginx-core
Suggested packages:
libgd-tools fcgiwrap nginx-doc ssl-cert
The following NEW packages will be installed:
fontconfig-config fonts-dejavu-core libfontconfig1 libgd3 libjbig0
libjpeg-turbo8 libjpeg8 libnginx-mod-http-image-filter
libnginx-mod-http-xslt-filter libnginx-mod-mail libnginx-mod-stream libtiff5
libwebp6 libxpm4 nginx nginx-common nginx-core
0 upgraded, 17 newly installed, 0 to remove and 41 not upgraded.
Need to get 2432 kB of archives.
After this operation, 7891 kB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 fonts-dejavu-core all 2.37-1 [1041 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 fontconfig-config all 2.13.1-2ubuntu3 [28.8 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libfontconfig1 amd64 2.13.1-2ubuntu3 [114 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libjpeg-turbo8 amd64 2.0.3-0ubuntu1.20.04.1 [117 kB]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libjpeg8 amd64 8c-2ubuntu8 [2194 B]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libjbig0 amd64 2.1-3.1build1 [26.7 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libwebp6 amd64 0.6.1-2ubuntu0.20.04.1 [185 kB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libtiff5 amd64 4.1.0+git191117-2ubuntu0.20.04.2 [162 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libxpm4 amd64 1:3.5.12-1 [34.0 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libgd3 amd64 2.2.5-5.2ubuntu2.1 [118 kB]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 nginx-common all 1.18.0-0ubuntu1.2 [37.5 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libnginx-mod-http-image-filter amd64 1.18.0-0ubuntu1.2 [14.4 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libnginx-mod-http-xslt-filter amd64 1.18.0-0ubuntu1.2 [12.7 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libnginx-mod-mail amd64 1.18.0-0ubuntu1.2 [42.5 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libnginx-mod-stream amd64 1.18.0-0ubuntu1.2 [67.3 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 nginx-core amd64 1.18.0-0ubuntu1.2 [425 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 nginx all 1.18.0-0ubuntu1.2 [3620 B]
Fetched 2432 kB in 0s (23.8 MB/s)
Preconfiguring packages ...
Selecting previously unselected package fonts-dejavu-core.
(Reading database ... 63895 files and directories currently installed.)
Preparing to unpack .../00-fonts-dejavu-core_2.37-1_all.deb ...
Unpacking fonts-dejavu-core (2.37-1) ...
Selecting previously unselected package fontconfig-config.
Preparing to unpack .../01-fontconfig-config_2.13.1-2ubuntu3_all.deb ...
Unpacking fontconfig-config (2.13.1-2ubuntu3) ...
Selecting previously unselected package libfontconfig1:amd64.
Preparing to unpack .../02-libfontconfig1_2.13.1-2ubuntu3_amd64.deb ...
Unpacking libfontconfig1:amd64 (2.13.1-2ubuntu3) ...
Selecting previously unselected package libjpeg-turbo8:amd64.
Preparing to unpack .../03-libjpeg-turbo8_2.0.3-0ubuntu1.20.04.1_amd64.deb ...
Unpacking libjpeg-turbo8:amd64 (2.0.3-0ubuntu1.20.04.1) ...
Selecting previously unselected package libjpeg8:amd64.
Preparing to unpack .../04-libjpeg8_8c-2ubuntu8_amd64.deb ...
Unpacking libjpeg8:amd64 (8c-2ubuntu8) ...
Selecting previously unselected package libjbig0:amd64.
Preparing to unpack .../05-libjbig0_2.1-3.1build1_amd64.deb ...
Unpacking libjbig0:amd64 (2.1-3.1build1) ...
Selecting previously unselected package libwebp6:amd64.
Preparing to unpack .../06-libwebp6_0.6.1-2ubuntu0.20.04.1_amd64.deb ...
Unpacking libwebp6:amd64 (0.6.1-2ubuntu0.20.04.1) ...
Selecting previously unselected package libtiff5:amd64.
Preparing to unpack .../07-libtiff5_4.1.0+git191117-2ubuntu0.20.04.2_amd64.deb ...
Unpacking libtiff5:amd64 (4.1.0+git191117-2ubuntu0.20.04.2) ...
Selecting previously unselected package libxpm4:amd64.
Preparing to unpack .../08-libxpm4_1%3a3.5.12-1_amd64.deb ...
Unpacking libxpm4:amd64 (1:3.5.12-1) ...
Selecting previously unselected package libgd3:amd64.
Preparing to unpack .../09-libgd3_2.2.5-5.2ubuntu2.1_amd64.deb ...
Unpacking libgd3:amd64 (2.2.5-5.2ubuntu2.1) ...
Selecting previously unselected package nginx-common.
Preparing to unpack .../10-nginx-common_1.18.0-0ubuntu1.2_all.deb ...
Unpacking nginx-common (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package libnginx-mod-http-image-filter.
Preparing to unpack .../11-libnginx-mod-http-image-filter_1.18.0-0ubuntu1.2_amd64.deb ...
Unpacking libnginx-mod-http-image-filter (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package libnginx-mod-http-xslt-filter.
Preparing to unpack .../12-libnginx-mod-http-xslt-filter_1.18.0-0ubuntu1.2_amd64.deb ...
Unpacking libnginx-mod-http-xslt-filter (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package libnginx-mod-mail.
Preparing to unpack .../13-libnginx-mod-mail_1.18.0-0ubuntu1.2_amd64.deb ...
Unpacking libnginx-mod-mail (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package libnginx-mod-stream.
Preparing to unpack .../14-libnginx-mod-stream_1.18.0-0ubuntu1.2_amd64.deb ...
Unpacking libnginx-mod-stream (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package nginx-core.
Preparing to unpack .../15-nginx-core_1.18.0-0ubuntu1.2_amd64.deb ...
Unpacking nginx-core (1.18.0-0ubuntu1.2) ...
Selecting previously unselected package nginx.
Preparing to unpack .../16-nginx_1.18.0-0ubuntu1.2_all.deb ...
Unpacking nginx (1.18.0-0ubuntu1.2) ...
Setting up libxpm4:amd64 (1:3.5.12-1) ...
Setting up nginx-common (1.18.0-0ubuntu1.2) ...
Created symlink /etc/systemd/system/multi-user.target.wants/nginx.service → /lib/systemd/system/nginx.service.
Setting up libjbig0:amd64 (2.1-3.1build1) ...
Setting up libnginx-mod-http-xslt-filter (1.18.0-0ubuntu1.2) ...
Setting up libwebp6:amd64 (0.6.1-2ubuntu0.20.04.1) ...
Setting up fonts-dejavu-core (2.37-1) ...
Setting up libjpeg-turbo8:amd64 (2.0.3-0ubuntu1.20.04.1) ...
Setting up libjpeg8:amd64 (8c-2ubuntu8) ...
Setting up libnginx-mod-mail (1.18.0-0ubuntu1.2) ...
Setting up fontconfig-config (2.13.1-2ubuntu3) ...
Setting up libnginx-mod-stream (1.18.0-0ubuntu1.2) ...
Setting up libtiff5:amd64 (4.1.0+git191117-2ubuntu0.20.04.2) ...
Setting up libfontconfig1:amd64 (2.13.1-2ubuntu3) ...
Setting up libgd3:amd64 (2.2.5-5.2ubuntu2.1) ...
Setting up libnginx-mod-http-image-filter (1.18.0-0ubuntu1.2) ...
Setting up nginx-core (1.18.0-0ubuntu1.2) ...
Setting up nginx (1.18.0-0ubuntu1.2) ...
Processing triggers for ufw (0.36-6ubuntu1) ...
Processing triggers for systemd (245.4-4ubuntu3.13) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.2) ...
ubuntu@ip-172-31-21-73:~$ sudo apt install mysql-server
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
libcgi-fast-perl libcgi-pm-perl libencode-locale-perl libevent-core-2.1-7
libevent-pthreads-2.1-7 libfcgi-perl libhtml-parser-perl libhtml-tagset-perl
libhtml-template-perl libhttp-date-perl libhttp-message-perl libio-html-perl
liblwp-mediatypes-perl libmecab2 libtimedate-perl liburi-perl mecab-ipadic
mecab-ipadic-utf8 mecab-utils mysql-client-8.0 mysql-client-core-8.0
mysql-common mysql-server-8.0 mysql-server-core-8.0
Suggested packages:
libdata-dump-perl libipc-sharedcache-perl libwww-perl mailx tinyca
The following NEW packages will be installed:
libcgi-fast-perl libcgi-pm-perl libencode-locale-perl libevent-core-2.1-7
libevent-pthreads-2.1-7 libfcgi-perl libhtml-parser-perl libhtml-tagset-perl
libhtml-template-perl libhttp-date-perl libhttp-message-perl libio-html-perl
liblwp-mediatypes-perl libmecab2 libtimedate-perl liburi-perl mecab-ipadic
mecab-ipadic-utf8 mecab-utils mysql-client-8.0 mysql-client-core-8.0
mysql-common mysql-server mysql-server-8.0 mysql-server-core-8.0
0 upgraded, 25 newly installed, 0 to remove and 41 not upgraded.
Need to get 31.9 MB of archives.
After this operation, 263 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 mysql-common all 5.8+1.0.5ubuntu2 [7496 B]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-client-core-8.0 amd64 8.0.27-0ubuntu0.20.04.1 [4423 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-client-8.0 amd64 8.0.27-0ubuntu0.20.04.1 [22.0 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libevent-core-2.1-7 amd64 2.1.11-stable-1 [89.1 kB]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libevent-pthreads-2.1-7 amd64 2.1.11-stable-1 [7372 B]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libmecab2 amd64 0.996-10build1 [233 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server-core-8.0 amd64 8.0.27-0ubuntu0.20.04.1 [18.4 MB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server-8.0 amd64 8.0.27-0ubuntu0.20.04.1 [1313 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libhtml-tagset-perl all 3.20-4 [12.5 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 liburi-perl all 1.76-2 [77.5 kB]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libhtml-parser-perl amd64 3.72-5 [86.3 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libcgi-pm-perl all 4.46-1 [186 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libfcgi-perl amd64 0.79-1 [33.1 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libcgi-fast-perl all 1:2.15-1 [10.5 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libencode-locale-perl all 1.05-1 [12.3 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libhtml-template-perl all 2.97-1 [59.0 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libtimedate-perl all 2.3200-1 [34.0 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libhttp-date-perl all 6.05-1 [9920 B]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libio-html-perl all 1.001-1 [14.9 kB]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 liblwp-mediatypes-perl all 6.04-1 [19.5 kB]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libhttp-message-perl all 6.22-1 [76.1 kB]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 mecab-utils amd64 0.996-10build1 [4912 B]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 mecab-ipadic all 2.7.0-20070801+main-2.1 [6714 kB]
Get:24 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 mecab-ipadic-utf8 all 2.7.0-20070801+main-2.1 [4380 B]
Get:25 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 mysql-server all 8.0.27-0ubuntu0.20.04.1 [9548 B]
Fetched 31.9 MB in 1s (52.1 MB/s)
Preconfiguring packages ...
Selecting previously unselected package mysql-common.
(Reading database ... 64122 files and directories currently installed.)
Preparing to unpack .../0-mysql-common_5.8+1.0.5ubuntu2_all.deb ...
Unpacking mysql-common (5.8+1.0.5ubuntu2) ...
Selecting previously unselected package mysql-client-core-8.0.
Preparing to unpack .../1-mysql-client-core-8.0_8.0.27-0ubuntu0.20.04.1_amd64.deb ...
Unpacking mysql-client-core-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Selecting previously unselected package mysql-client-8.0.
Preparing to unpack .../2-mysql-client-8.0_8.0.27-0ubuntu0.20.04.1_amd64.deb ...
Unpacking mysql-client-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Selecting previously unselected package libevent-core-2.1-7:amd64.
Preparing to unpack .../3-libevent-core-2.1-7_2.1.11-stable-1_amd64.deb ...
Unpacking libevent-core-2.1-7:amd64 (2.1.11-stable-1) ...
Selecting previously unselected package libevent-pthreads-2.1-7:amd64.
Preparing to unpack .../4-libevent-pthreads-2.1-7_2.1.11-stable-1_amd64.deb ...
Unpacking libevent-pthreads-2.1-7:amd64 (2.1.11-stable-1) ...
Selecting previously unselected package libmecab2:amd64.
Preparing to unpack .../5-libmecab2_0.996-10build1_amd64.deb ...
Unpacking libmecab2:amd64 (0.996-10build1) ...
Selecting previously unselected package mysql-server-core-8.0.
Preparing to unpack .../6-mysql-server-core-8.0_8.0.27-0ubuntu0.20.04.1_amd64.deb ...
Unpacking mysql-server-core-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Setting up mysql-common (5.8+1.0.5ubuntu2) ...
update-alternatives: using /etc/mysql/my.cnf.fallback to provide /etc/mysql/my.cnf (my.cnf) in auto mode
Selecting previously unselected package mysql-server-8.0.
(Reading database ... 64344 files and directories currently installed.)
Preparing to unpack .../00-mysql-server-8.0_8.0.27-0ubuntu0.20.04.1_amd64.deb ...
Unpacking mysql-server-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Selecting previously unselected package libhtml-tagset-perl.
Preparing to unpack .../01-libhtml-tagset-perl_3.20-4_all.deb ...
Unpacking libhtml-tagset-perl (3.20-4) ...
Selecting previously unselected package liburi-perl.
Preparing to unpack .../02-liburi-perl_1.76-2_all.deb ...
Unpacking liburi-perl (1.76-2) ...
Selecting previously unselected package libhtml-parser-perl.
Preparing to unpack .../03-libhtml-parser-perl_3.72-5_amd64.deb ...
Unpacking libhtml-parser-perl (3.72-5) ...
Selecting previously unselected package libcgi-pm-perl.
Preparing to unpack .../04-libcgi-pm-perl_4.46-1_all.deb ...
Unpacking libcgi-pm-perl (4.46-1) ...
Selecting previously unselected package libfcgi-perl.
Preparing to unpack .../05-libfcgi-perl_0.79-1_amd64.deb ...
Unpacking libfcgi-perl (0.79-1) ...
Selecting previously unselected package libcgi-fast-perl.
Preparing to unpack .../06-libcgi-fast-perl_1%3a2.15-1_all.deb ...
Unpacking libcgi-fast-perl (1:2.15-1) ...
Selecting previously unselected package libencode-locale-perl.
Preparing to unpack .../07-libencode-locale-perl_1.05-1_all.deb ...
Unpacking libencode-locale-perl (1.05-1) ...
Selecting previously unselected package libhtml-template-perl.
Preparing to unpack .../08-libhtml-template-perl_2.97-1_all.deb ...
Unpacking libhtml-template-perl (2.97-1) ...
Selecting previously unselected package libtimedate-perl.
Preparing to unpack .../09-libtimedate-perl_2.3200-1_all.deb ...
Unpacking libtimedate-perl (2.3200-1) ...
Selecting previously unselected package libhttp-date-perl.
Preparing to unpack .../10-libhttp-date-perl_6.05-1_all.deb ...
Unpacking libhttp-date-perl (6.05-1) ...
Selecting previously unselected package libio-html-perl.
Preparing to unpack .../11-libio-html-perl_1.001-1_all.deb ...
Unpacking libio-html-perl (1.001-1) ...
Selecting previously unselected package liblwp-mediatypes-perl.
Preparing to unpack .../12-liblwp-mediatypes-perl_6.04-1_all.deb ...
Unpacking liblwp-mediatypes-perl (6.04-1) ...
Selecting previously unselected package libhttp-message-perl.
Preparing to unpack .../13-libhttp-message-perl_6.22-1_all.deb ...
Unpacking libhttp-message-perl (6.22-1) ...
Selecting previously unselected package mecab-utils.
Preparing to unpack .../14-mecab-utils_0.996-10build1_amd64.deb ...
Unpacking mecab-utils (0.996-10build1) ...
Selecting previously unselected package mecab-ipadic.
Preparing to unpack .../15-mecab-ipadic_2.7.0-20070801+main-2.1_all.deb ...
Unpacking mecab-ipadic (2.7.0-20070801+main-2.1) ...
Selecting previously unselected package mecab-ipadic-utf8.
Preparing to unpack .../16-mecab-ipadic-utf8_2.7.0-20070801+main-2.1_all.deb ...
Unpacking mecab-ipadic-utf8 (2.7.0-20070801+main-2.1) ...
Selecting previously unselected package mysql-server.
Preparing to unpack .../17-mysql-server_8.0.27-0ubuntu0.20.04.1_all.deb ...
Unpacking mysql-server (8.0.27-0ubuntu0.20.04.1) ...
Setting up libmecab2:amd64 (0.996-10build1) ...
Setting up mysql-client-core-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Setting up libhtml-tagset-perl (3.20-4) ...
Setting up liblwp-mediatypes-perl (6.04-1) ...
Setting up libencode-locale-perl (1.05-1) ...
Setting up mecab-utils (0.996-10build1) ...
Setting up libevent-core-2.1-7:amd64 (2.1.11-stable-1) ...
Setting up libio-html-perl (1.001-1) ...
Setting up libtimedate-perl (2.3200-1) ...
Setting up mysql-client-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Setting up libfcgi-perl (0.79-1) ...
Setting up liburi-perl (1.76-2) ...
Setting up libevent-pthreads-2.1-7:amd64 (2.1.11-stable-1) ...
Setting up libhttp-date-perl (6.05-1) ...
Setting up mecab-ipadic (2.7.0-20070801+main-2.1) ...
Compiling IPA dictionary for Mecab. This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################|
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
emitting double-array: 100% |###########################################|
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix : 100% |###########################################|

done!
update-alternatives: using /var/lib/mecab/dic/ipadic to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up mysql-server-core-8.0 (8.0.27-0ubuntu0.20.04.1) ...
Setting up mecab-ipadic-utf8 (2.7.0-20070801+main-2.1) ...
Compiling IPA dictionary for Mecab. This takes long time...
reading /usr/share/mecab/dic/ipadic/unk.def ... 40
emitting double-array: 100% |###########################################|
/usr/share/mecab/dic/ipadic/model.def is not found. skipped.
reading /usr/share/mecab/dic/ipadic/Noun.org.csv ... 16668
reading /usr/share/mecab/dic/ipadic/Adnominal.csv ... 135
reading /usr/share/mecab/dic/ipadic/Conjunction.csv ... 171
reading /usr/share/mecab/dic/ipadic/Adj.csv ... 27210
reading /usr/share/mecab/dic/ipadic/Postp-col.csv ... 91
reading /usr/share/mecab/dic/ipadic/Noun.adjv.csv ... 3328
reading /usr/share/mecab/dic/ipadic/Noun.adverbal.csv ... 795
reading /usr/share/mecab/dic/ipadic/Interjection.csv ... 252
reading /usr/share/mecab/dic/ipadic/Noun.nai.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.verbal.csv ... 12146
reading /usr/share/mecab/dic/ipadic/Prefix.csv ... 221
reading /usr/share/mecab/dic/ipadic/Symbol.csv ... 208
reading /usr/share/mecab/dic/ipadic/Noun.number.csv ... 42
reading /usr/share/mecab/dic/ipadic/Noun.place.csv ... 72999
reading /usr/share/mecab/dic/ipadic/Verb.csv ... 130750
reading /usr/share/mecab/dic/ipadic/Noun.others.csv ... 151
reading /usr/share/mecab/dic/ipadic/Noun.csv ... 60477
reading /usr/share/mecab/dic/ipadic/Suffix.csv ... 1393
reading /usr/share/mecab/dic/ipadic/Noun.demonst.csv ... 120
reading /usr/share/mecab/dic/ipadic/Noun.name.csv ... 34202
reading /usr/share/mecab/dic/ipadic/Postp.csv ... 146
reading /usr/share/mecab/dic/ipadic/Filler.csv ... 19
reading /usr/share/mecab/dic/ipadic/Auxil.csv ... 199
reading /usr/share/mecab/dic/ipadic/Others.csv ... 2
reading /usr/share/mecab/dic/ipadic/Adverb.csv ... 3032
reading /usr/share/mecab/dic/ipadic/Noun.proper.csv ... 27328
emitting double-array: 100% |###########################################|
reading /usr/share/mecab/dic/ipadic/matrix.def ... 1316x1316
emitting matrix : 100% |###########################################|

done!
update-alternatives: using /var/lib/mecab/dic/ipadic-utf8 to provide /var/lib/mecab/dic/debian (mecab-dictionary) in auto mode
Setting up libhtml-parser-perl (3.72-5) ...
Setting up libhttp-message-perl (6.22-1) ...
Setting up mysql-server-8.0 (8.0.27-0ubuntu0.20.04.1) ...
update-alternatives: using /etc/mysql/mysql.cnf to provide /etc/mysql/my.cnf (my.cnf) in auto mode
Renaming removed key_buffer and myisam-recover options (if present)
mysqld will log errors to /var/log/mysql/error.log
mysqld is running as pid 2667
Created symlink /etc/systemd/system/multi-user.target.wants/mysql.service → /lib/systemd/system/mysql.service.
Setting up libcgi-pm-perl (4.46-1) ...
Setting up libhtml-template-perl (2.97-1) ...
Setting up mysql-server (8.0.27-0ubuntu0.20.04.1) ...
Setting up libcgi-fast-perl (1:2.15-1) ...
Processing triggers for systemd (245.4-4ubuntu3.13) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.2) ...
ubuntu@ip-172-31-21-73:~$ sudo mysql_secure_installation

Securing the MySQL server deployment.

Connecting to MySQL using a blank password.

VALIDATE PASSWORD COMPONENT can be used to test passwords
and improve security. It checks the strength of password
and allows the users to set only those passwords which are
secure enough. Would you like to setup VALIDATE PASSWORD component?

Press y|Y for Yes, any other key for No: n
Please set the password for root here.

New password:

Re-enter new password:
By default, a MySQL installation has an anonymous user,
allowing anyone to log into MySQL without having to have
a user account created for them. This is intended only for
testing, and to make the installation go a bit smoother.
You should remove them before moving into a production
environment.

Remove anonymous users? (Press y|Y for Yes, any other key for No) :y
Success.

Normally, root should only be allowed to connect from
'localhost'. This ensures that someone cannot guess at
the root password from the network.

Disallow root login remotely? (Press y|Y for Yes, any other key for No) : y
Success.

By default, MySQL comes with a database named 'test' that
anyone can access. This is also intended only for testing,
and should be removed before moving into a production
environment.

Remove test database and access to it? (Press y|Y for Yes, any other key for No) : y

- Dropping test database...
  Success.

- Removing privileges on test database...
  Success.

Reloading the privilege tables will ensure that all changes
made so far will take effect immediately.

Reload privilege tables now? (Press y|Y for Yes, any other key for No) : y
Success.

All done!
ubuntu@ip-172-31-21-73:~$ sudo msql
sudo: msql: command not found
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 10
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> exit
Bye
ubuntu@ip-172-31-21-73:~$ sudo apt install php libapache2-mod-php php-mysql
Reading package lists... Done
Building dependency tree
Reading state information... Done
The following additional packages will be installed:
apache2 apache2-bin apache2-data apache2-utils libapache2-mod-php7.4 libapr1
libaprutil1 libaprutil1-dbd-sqlite3 libaprutil1-ldap libjansson4 liblua5.2-0
php-common php7.4 php7.4-cli php7.4-common php7.4-json php7.4-mysql
php7.4-opcache php7.4-readline ssl-cert
Suggested packages:
apache2-doc apache2-suexec-pristine | apache2-suexec-custom www-browser
php-pear openssl-blacklist
The following NEW packages will be installed:
apache2 apache2-bin apache2-data apache2-utils libapache2-mod-php
libapache2-mod-php7.4 libapr1 libaprutil1 libaprutil1-dbd-sqlite3
libaprutil1-ldap libjansson4 liblua5.2-0 php php-common php-mysql php7.4
php7.4-cli php7.4-common php7.4-json php7.4-mysql php7.4-opcache
php7.4-readline ssl-cert
0 upgraded, 23 newly installed, 0 to remove and 41 not upgraded.
Need to get 6012 kB of archives.
After this operation, 26.6 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libapr1 amd64 1.6.5-1ubuntu1 [91.4 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1 amd64 1.6.1-4ubuntu2 [84.7 kB]
Get:3 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-dbd-sqlite3 amd64 1.6.1-4ubuntu2 [10.5 kB]
Get:4 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libaprutil1-ldap amd64 1.6.1-4ubuntu2 [8736 B]
Get:5 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libjansson4 amd64 2.12-1build1 [28.9 kB]
Get:6 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 liblua5.2-0 amd64 5.2.4-1.1build3 [106 kB]
Get:7 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-bin amd64 2.4.41-4ubuntu3.9 [1180 kB]
Get:8 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-data all 2.4.41-4ubuntu3.9 [159 kB]
Get:9 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2-utils amd64 2.4.41-4ubuntu3.9 [84.3 kB]
Get:10 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 apache2 amd64 2.4.41-4ubuntu3.9 [95.5 kB]
Get:11 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 php-common all 2:75 [11.9 kB]
Get:12 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-common amd64 7.4.3-4ubuntu2.8 [981 kB]
Get:13 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-json amd64 7.4.3-4ubuntu2.8 [19.2 kB]
Get:14 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-opcache amd64 7.4.3-4ubuntu2.8 [198 kB]
Get:15 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-readline amd64 7.4.3-4ubuntu2.8 [12.6 kB]
Get:16 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-cli amd64 7.4.3-4ubuntu2.8 [1421 kB]
Get:17 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 libapache2-mod-php7.4 amd64 7.4.3-4ubuntu2.8 [1364 kB]
Get:18 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 libapache2-mod-php all 2:7.4+75 [2836 B]
Get:19 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4 all 7.4.3-4ubuntu2.8 [9236 B]
Get:20 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 php all 2:7.4+75 [2712 B]
Get:21 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/main amd64 php7.4-mysql amd64 7.4.3-4ubuntu2.8 [121 kB]
Get:22 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 php-mysql all 2:7.4+75 [2000 B]
Get:23 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/main amd64 ssl-cert all 1.0.39 [17.0 kB]
Fetched 6012 kB in 0s (38.0 MB/s)
Preconfiguring packages ...
Selecting previously unselected package libapr1:amd64.
(Reading database ... 64714 files and directories currently installed.)
Preparing to unpack .../00-libapr1_1.6.5-1ubuntu1_amd64.deb ...
Unpacking libapr1:amd64 (1.6.5-1ubuntu1) ...
Selecting previously unselected package libaprutil1:amd64.
Preparing to unpack .../01-libaprutil1_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libaprutil1-dbd-sqlite3:amd64.
Preparing to unpack .../02-libaprutil1-dbd-sqlite3_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libaprutil1-ldap:amd64.
Preparing to unpack .../03-libaprutil1-ldap_1.6.1-4ubuntu2_amd64.deb ...
Unpacking libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Selecting previously unselected package libjansson4:amd64.
Preparing to unpack .../04-libjansson4_2.12-1build1_amd64.deb ...
Unpacking libjansson4:amd64 (2.12-1build1) ...
Selecting previously unselected package liblua5.2-0:amd64.
Preparing to unpack .../05-liblua5.2-0_5.2.4-1.1build3_amd64.deb ...
Unpacking liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Selecting previously unselected package apache2-bin.
Preparing to unpack .../06-apache2-bin_2.4.41-4ubuntu3.9_amd64.deb ...
Unpacking apache2-bin (2.4.41-4ubuntu3.9) ...
Selecting previously unselected package apache2-data.
Preparing to unpack .../07-apache2-data_2.4.41-4ubuntu3.9_all.deb ...
Unpacking apache2-data (2.4.41-4ubuntu3.9) ...
Selecting previously unselected package apache2-utils.
Preparing to unpack .../08-apache2-utils_2.4.41-4ubuntu3.9_amd64.deb ...
Unpacking apache2-utils (2.4.41-4ubuntu3.9) ...
Selecting previously unselected package apache2.
Preparing to unpack .../09-apache2_2.4.41-4ubuntu3.9_amd64.deb ...
Unpacking apache2 (2.4.41-4ubuntu3.9) ...
Selecting previously unselected package php-common.
Preparing to unpack .../10-php-common_2%3a75_all.deb ...
Unpacking php-common (2:75) ...
Selecting previously unselected package php7.4-common.
Preparing to unpack .../11-php7.4-common_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-common (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php7.4-json.
Preparing to unpack .../12-php7.4-json_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-json (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php7.4-opcache.
Preparing to unpack .../13-php7.4-opcache_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-opcache (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php7.4-readline.
Preparing to unpack .../14-php7.4-readline_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-readline (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php7.4-cli.
Preparing to unpack .../15-php7.4-cli_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-cli (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package libapache2-mod-php7.4.
Preparing to unpack .../16-libapache2-mod-php7.4_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking libapache2-mod-php7.4 (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package libapache2-mod-php.
Preparing to unpack .../17-libapache2-mod-php_2%3a7.4+75_all.deb ...
Unpacking libapache2-mod-php (2:7.4+75) ...
Selecting previously unselected package php7.4.
Preparing to unpack .../18-php7.4_7.4.3-4ubuntu2.8_all.deb ...
Unpacking php7.4 (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php.
Preparing to unpack .../19-php_2%3a7.4+75_all.deb ...
Unpacking php (2:7.4+75) ...
Selecting previously unselected package php7.4-mysql.
Preparing to unpack .../20-php7.4-mysql_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-mysql (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php-mysql.
Preparing to unpack .../21-php-mysql_2%3a7.4+75_all.deb ...
Unpacking php-mysql (2:7.4+75) ...
Selecting previously unselected package ssl-cert.
Preparing to unpack .../22-ssl-cert_1.0.39_all.deb ...
Unpacking ssl-cert (1.0.39) ...
Setting up php-common (2:75) ...
Created symlink /etc/systemd/system/timers.target.wants/phpsessionclean.timer → /lib/systemd/system/phpsessionclean.timer.
Setting up php7.4-common (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/mods-available/calendar.ini with new version

Creating config file /etc/php/7.4/mods-available/ctype.ini with new version

Creating config file /etc/php/7.4/mods-available/exif.ini with new version

Creating config file /etc/php/7.4/mods-available/fileinfo.ini with new version

Creating config file /etc/php/7.4/mods-available/ffi.ini with new version

Creating config file /etc/php/7.4/mods-available/ftp.ini with new version

Creating config file /etc/php/7.4/mods-available/gettext.ini with new version

Creating config file /etc/php/7.4/mods-available/iconv.ini with new version

Creating config file /etc/php/7.4/mods-available/pdo.ini with new version

Creating config file /etc/php/7.4/mods-available/phar.ini with new version

Creating config file /etc/php/7.4/mods-available/posix.ini with new version

Creating config file /etc/php/7.4/mods-available/shmop.ini with new version

Creating config file /etc/php/7.4/mods-available/sockets.ini with new version

Creating config file /etc/php/7.4/mods-available/sysvmsg.ini with new version

Creating config file /etc/php/7.4/mods-available/sysvsem.ini with new version

Creating config file /etc/php/7.4/mods-available/sysvshm.ini with new version

Creating config file /etc/php/7.4/mods-available/tokenizer.ini with new version
Setting up php7.4-mysql (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/mods-available/mysqlnd.ini with new version

Creating config file /etc/php/7.4/mods-available/mysqli.ini with new version

Creating config file /etc/php/7.4/mods-available/pdo_mysql.ini with new version
Setting up libapr1:amd64 (1.6.5-1ubuntu1) ...
Setting up php7.4-readline (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/mods-available/readline.ini with new version
Setting up libjansson4:amd64 (2.12-1build1) ...
Setting up ssl-cert (1.0.39) ...
Setting up liblua5.2-0:amd64 (5.2.4-1.1build3) ...
Setting up php7.4-opcache (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/mods-available/opcache.ini with new version
Setting up apache2-data (2.4.41-4ubuntu3.9) ...
Setting up libaprutil1:amd64 (1.6.1-4ubuntu2) ...
Setting up php7.4-json (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/mods-available/json.ini with new version
Setting up php-mysql (2:7.4+75) ...
Setting up php7.4-cli (7.4.3-4ubuntu2.8) ...
update-alternatives: using /usr/bin/php7.4 to provide /usr/bin/php (php) in auto mode
update-alternatives: using /usr/bin/phar7.4 to provide /usr/bin/phar (phar) in auto mode
update-alternatives: using /usr/bin/phar.phar7.4 to provide /usr/bin/phar.phar (phar.phar) in auto mode

Creating config file /etc/php/7.4/cli/php.ini with new version
Setting up libaprutil1-ldap:amd64 (1.6.1-4ubuntu2) ...
Setting up libaprutil1-dbd-sqlite3:amd64 (1.6.1-4ubuntu2) ...
Setting up apache2-utils (2.4.41-4ubuntu3.9) ...
Setting up apache2-bin (2.4.41-4ubuntu3.9) ...
Setting up libapache2-mod-php7.4 (7.4.3-4ubuntu2.8) ...
Package apache2 is not configured yet. Will defer actions by package libapache2-mod-php7.4.

Creating config file /etc/php/7.4/apache2/php.ini with new version
No module matches
Setting up apache2 (2.4.41-4ubuntu3.9) ...
Enabling module mpm_event.
Enabling module authz_core.
Enabling module authz_host.
Enabling module authn_core.
Enabling module auth_basic.
Enabling module access_compat.
Enabling module authn_file.
Enabling module authz_user.
Enabling module alias.
Enabling module dir.
Enabling module autoindex.
Enabling module env.
Enabling module mime.
Enabling module negotiation.
Enabling module setenvif.
Enabling module filter.
Enabling module deflate.
Enabling module status.
Enabling module reqtimeout.
Enabling conf charset.
Enabling conf localized-error-pages.
Enabling conf other-vhosts-access-log.
Enabling conf security.
Enabling conf serve-cgi-bin.
Enabling site 000-default.
info: Switch to mpm prefork for package libapache2-mod-php7.4
Module mpm_event disabled.
Enabling module mpm_prefork.
info: Executing deferred 'a2enmod php7.4' for package libapache2-mod-php7.4
Enabling module php7.4.
Created symlink /etc/systemd/system/multi-user.target.wants/apache2.service → /lib/systemd/system/apache2.service.
Created symlink /etc/systemd/system/multi-user.target.wants/apache-htcacheclean.service → /lib/systemd/system/apache-htcacheclean.service.
Job for apache2.service failed because the control process exited with error code.
See "systemctl status apache2.service" and "journalctl -xe" for details.
invoke-rc.d: initscript apache2, action "start" failed.
● apache2.service - The Apache HTTP Server
Loaded: loaded (/lib/systemd/system/apache2.service; enabled; vendor preset: enabled)
Active: failed (Result: exit-code) since Tue 2022-02-01 23:23:06 UTC; 9ms ago
Docs: https://httpd.apache.org/docs/2.4/
Process: 11324 ExecStart=/usr/sbin/apachectl start (code=exited, status=1/FAILURE)

Feb 01 23:23:06 ip-172-31-21-73 systemd[1]: Starting The Apache HTTP Server...
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11327]: (98)Address already in use: AH00072: make_sock: could not bind to address [::]:80
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11327]: (98)Address already in use: AH00072: make_sock: could not bind to address 0.0.0.0:80
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11327]: no listening sockets available, shutting down
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11327]: AH00015: Unable to open logs
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11324]: Action 'start' failed.
Feb 01 23:23:06 ip-172-31-21-73 apachectl[11324]: The Apache error log may have more information.
Feb 01 23:23:06 ip-172-31-21-73 systemd[1]: apache2.service: Control process exited, code=exited, status=1/FAILURE
Feb 01 23:23:06 ip-172-31-21-73 systemd[1]: apache2.service: Failed with result 'exit-code'.
Feb 01 23:23:06 ip-172-31-21-73 systemd[1]: Failed to start The Apache HTTP Server.
Setting up php7.4 (7.4.3-4ubuntu2.8) ...
Setting up libapache2-mod-php (2:7.4+75) ...
Setting up php (2:7.4+75) ...
Processing triggers for ufw (0.36-6ubuntu1) ...
Processing triggers for systemd (245.4-4ubuntu3.13) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for libc-bin (2.31-0ubuntu9.2) ...
Processing triggers for php7.4-cli (7.4.3-4ubuntu2.8) ...
Processing triggers for libapache2-mod-php7.4 (7.4.3-4ubuntu2.8) ...
ubuntu@ip-172-31-21-73:~$ sudo apt install php-fpm php-mysql
Reading package lists... Done
Building dependency tree
Reading state information... Done
php-mysql is already the newest version (2:7.4+75).
Suggested packages:
php-pear
The following NEW packages will be installed:
php-fpm php7.4-fpm
0 upgraded, 2 newly installed, 0 to remove and 41 not upgraded.
Need to get 1437 kB of archives.
After this operation, 4877 kB of additional disk space will be used.
Get:1 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal-updates/universe amd64 php7.4-fpm amd64 7.4.3-4ubuntu2.8 [1434 kB]
Get:2 http://us-east-1.ec2.archive.ubuntu.com/ubuntu focal/universe amd64 php-fpm all 2:7.4+75 [2792 B]
Fetched 1437 kB in 0s (33.4 MB/s)
Selecting previously unselected package php7.4-fpm.
(Reading database ... 65595 files and directories currently installed.)
Preparing to unpack .../php7.4-fpm_7.4.3-4ubuntu2.8_amd64.deb ...
Unpacking php7.4-fpm (7.4.3-4ubuntu2.8) ...
Selecting previously unselected package php-fpm.
Preparing to unpack .../php-fpm_2%3a7.4+75_all.deb ...
Unpacking php-fpm (2:7.4+75) ...
Setting up php7.4-fpm (7.4.3-4ubuntu2.8) ...

Creating config file /etc/php/7.4/fpm/php.ini with new version
NOTICE: Not enabling PHP 7.4 FPM by default.
NOTICE: To enable PHP 7.4 FPM in Apache2 do:
NOTICE: a2enmod proxy_fcgi setenvif
NOTICE: a2enconf php7.4-fpm
NOTICE: You are seeing this message because you have apache2 package installed.
Created symlink /etc/systemd/system/multi-user.target.wants/php7.4-fpm.service → /lib/systemd/system/php7.4-fpm.service.
Setting up php-fpm (2:7.4+75) ...
Processing triggers for man-db (2.9.1-1) ...
Processing triggers for systemd (245.4-4ubuntu3.13) ...
Processing triggers for php7.4-fpm (7.4.3-4ubuntu2.8) ...
NOTICE: Not enabling PHP 7.4 FPM by default.
NOTICE: To enable PHP 7.4 FPM in Apache2 do:
NOTICE: a2enmod proxy_fcgi setenvif
NOTICE: a2enconf php7.4-fpm
NOTICE: You are seeing this message because you have apache2 package installed.
ubuntu@ip-172-31-21-73:~$ sudo mkdir /var/www/projectLEMP
ubuntu@ip-172-31-21-73:~$ sudo chown -R $USER:$USER /var/www/projectLEMP
ubuntu@ip-172-31-21-73:~$ sudo nano /etc/nginx/sites-available/projectLEMP
ubuntu@ip-172-31-21-73:~$ sudo ln -s /etc/nginx/sites-available/projectLEMP /etc/nginx/sites-enabled/
ubuntu@ip-172-31-21-73:~$ sudo nginx -t
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
ubuntu@ip-172-31-21-73:~$
ubuntu@ip-172-31-21-73:~$ sudo unlink /etc/nginx/sites-enabled/default
ubuntu@ip-172-31-21-73:~$ sudo systemctl reload nginx
ubuntu@ip-172-31-21-73:~$ sudo nano /var/www/projectLEMP
ubuntu@ip-172-31-21-73:~$ sudo echo 'Hello LEMP from hostname' $(curl -s http://169.254.169.254/latest/meta-data/public-hostname) 'with public IP' $(curl -s http://169.254.169.254/latest/meta-data/public-ipv4) > /var/www/projectLEMP/index.html
ubuntu@ip-172-31-21-73:~$ sudo nano /var/www/projectLEMP/info.php
ubuntu@ip-172-31-21-73:~$ sudo rm /var/www/your_domain/info.php
rm: cannot remove '/var/www/your_domain/info.php': No such file or directory
ubuntu@ip-172-31-21-73:~$ sudo rm /var/www/your_domain/info.php
rm: cannot remove '/var/www/your_domain/info.php': No such file or directory
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 11
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> mysql> CREATE DATABASE `example_database`;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> CREATE DATABASE `example_database`' at line 1
mysql> mysql> CREATE DATABASE example_database;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> CREATE DATABASE example_database' at line 1
mysql> mysql> CREATE DATABASE example_database;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> CREATE DATABASE example_database' at line 1
mysql> mysql -V
-> Aborted
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 12
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> CREATE DATABASE `example_database`;
Query OK, 1 row affected (0.01 sec)

mysql> mysql> CREATE USER 'example_user'@'%' IDENTIFIED WITH mysql_native_password BY 'password';Sexywunmi123
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> CREATE USER 'example_user'@'%' IDENTIFIED WITH mysql_native_password BY ' at line 1
-> password
-> password
-> Aborted
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 13
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> CREATE DATABASE `example_database`;
ERROR 1007 (HY000): Can't create database 'example_database'; database exists
mysql> CREATE USER 'example_user'@'%' IDENTIFIED WITH mysql_native_password BY 'password';password
Query OK, 0 rows affected (0.01 sec)

    -> GRANT ALL ON example_database.* TO 'example_user'@'%';

ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'password
GRANT ALL ON example_database._ TO 'example_user'@'%'' at line 1
mysql> GRANT ALL ON example_database._ TO 'example_user'@'%';
Query OK, 0 rows affected (0.00 sec)

mysql> exit
Bye
ubuntu@ip-172-31-21-73:~$ mysql -u example_user -p
Enter password:
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 14
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> SHOW DATABASES;
+--------------------+
| Database |
+--------------------+
| example_database |
| information_schema |
+--------------------+
2 rows in set (0.01 sec)

mysql> CREATE TABLE example_database.todo_list (
-> mysql> item_id INT AUTO_INCREMENT,
-> mysql> content VARCHAR(255),
-> mysql> PRIMARY KEY(item_id)
-> mysql> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '> item_id INT AUTO_INCREMENT,
mysql> content VARCHAR(255),
mysql> PR' at line 2
mysql> CREATE TABLE example_database.todo_list (
-> mysql> item_id INT AUTO_INCREMENT,
-> mysql> content VARCHAR(255),
-> mysql> PRIMARY KEY(item_id)
-> mysql> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '> item_id INT AUTO_INCREMENT,
mysql> content VARCHAR(255),
mysql> PR' at line 2
mysql> CREATE TABLE example_database.todo_list ( mysql> item_id INT AUTO_INCREMENT, mysql> content VARCHAR(255), mysql> PRIMARY KEY(item_id) mysql> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '> item_id INT AUTO_INCREMENT, mysql> content VARCHAR(255), mysql> PR' at line 1
mysql> CREATE TABLE example_database.todo_list (
-> mysql> item_id INT AUTO_INCREMENT,
-> mysql> content VARCHAR(255),
-> mysql> PRIMARY KEY(item_id),
-> mysql> );
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near '> item_id INT AUTO_INCREMENT,
mysql> content VARCHAR(255),
mysql> PR' at line 2
mysql> CREATE TABLE example_database.todo_list
->
->
-> mysql> item_id INT AUTO_INCREMENT
->
->
->
->
->
->
->
->
->
->
-> Aborted
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 15
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show database;
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'database' at line 1
mysql> show databases
-> Aborted
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 16
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show databases;
+--------------------+
| Database |
+--------------------+
| example_database |
| information_schema |
| mysql |
| performance_schema |
| sys |
+--------------------+
5 rows in set (0.00 sec)

mysql> CREATE TABLE example_database.todo_list (
->
-> exit
->
->
-> '\c'
->
-> '\h'
->
->
->
-> Aborted
ubuntu@ip-172-31-21-73:~$ sudo mysql
Welcome to the MySQL monitor. Commands end with ; or \g.
Your MySQL connection id is 17
Server version: 8.0.27-0ubuntu0.20.04.1 (Ubuntu)

Copyright (c) 2000, 2021, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql> show databases;
+--------------------+
| Database |
+--------------------+
| example_database |
| information_schema |
| mysql |
| performance_schema |
| sys |
+--------------------+
5 rows in set (0.00 sec)

mysql> CREATE TABLE example_database.todo_list (item_id INT AUTO_INCREMENT, content VARCHAR(255), PRIMARY KEY(item_id));
Query OK, 0 rows affected (0.03 sec)

mysql> mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first important item");
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that corresponds to your MySQL server version for the right syntax to use near 'mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first import' at line 1
mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first important item");
Query OK, 1 row affected (0.01 sec)

mysql> SELECT \* FROM example_database.todo_list;
+---------+-------------------------+
| item_id | content |
+---------+-------------------------+
| 1 | My first important item |
+---------+-------------------------+
1 row in set (0.00 sec)

mysql> CREATE TABLE example_database.todo_list (item_id INT AUTO_INCREMENT);
ERROR 1050 (42S01): Table 'todo_list' already exists
mysql> SELECT \* FROM example_database.todo_list;
+---------+-------------------------+
| item_id | content |
+---------+-------------------------+
| 1 | My first important item |
+---------+-------------------------+
1 row in set (0.00 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first important item");
Query OK, 1 row affected (0.01 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("My first important item");
Query OK, 1 row affected (0.01 sec)

mysql> SELECT \* FROM example_database.todo_list;
+---------+-------------------------+
| item_id | content |
+---------+-------------------------+
| 1 | My first important item |
| 2 | My first important item |
| 3 | My first important item |
+---------+-------------------------+
3 rows in set (0.00 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("My second important item");
Query OK, 1 row affected (0.01 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("My third important item");
Query OK, 1 row affected (0.00 sec)

mysql> INSERT INTO example_database.todo_list (content) VALUES ("and this one more thing");
Query OK, 1 row affected (0.01 sec)

mysql> SELECT \* FROM example_database.todo_list;
+---------+--------------------------+
| item_id | content |
+---------+--------------------------+
| 1 | My first important item |
| 2 | My first important item |
| 3 | My first important item |
| 4 | My second important item |
| 5 | My third important item |
| 6 | and this one more thing |
+---------+--------------------------+
6 rows in set (0.00 sec)

mysql> exit
Bye
ubuntu@ip-172-31-21-73:~$ nano /var/www/projectLEMP/todo_list.php
