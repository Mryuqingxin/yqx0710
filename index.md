[root@jdu4e00u53f7 CV]# wget http://labfile.oss.aliyuncs.com/courses/624/cv-template.zip
--2017-07-25 09:59:13--  http://labfile.oss.aliyuncs.com/courses/624/cv-template.zip
Resolving labfile.oss.aliyuncs.com... 118.178.161.16
Connecting to labfile.oss.aliyuncs.com|118.178.161.16|:80... connected.
HTTP request sent, awaiting response... 200 OK
Length: 156602 (153K) [application/zip]
Saving to: “cv-template.zip”
 
100%[====================================================================>] 156,602     --.-K/s   in 0.1s    
 
2017-07-25 09:59:13 (1.26 MB/s) - “cv-template.zip” saved [156602/156602]
 
[root@jdu4e00u53f7 CV]# unzip cv-template.zip 
Archive:  cv-template.zip
   creating: cv-template/
  inflating: cv-template/.DS_Store   
   creating: __MACOSX/
   creating: __MACOSX/cv-template/
  inflating: __MACOSX/cv-template/._.DS_Store  
  inflating: cv-template/index.html  
   creating: cv-template/static/
  inflating: cv-template/static/.DS_Store  
   creating: __MACOSX/cv-template/static/
  inflating: __MACOSX/cv-template/static/._.DS_Store  
   creating: cv-template/static/css/
  inflating: cv-template/static/css/.DS_Store  
   creating: __MACOSX/cv-template/static/css/
  inflating: __MACOSX/cv-template/static/css/._.DS_Store  
  inflating: cv-template/static/css/style.css  
   creating: cv-template/static/fonts/
  inflating: cv-template/static/fonts/.DS_Store  
   creating: __MACOSX/cv-template/static/fonts/
  inflating: __MACOSX/cv-template/static/fonts/._.DS_Store  
  inflating: cv-template/static/fonts/demo.css  
  inflating: cv-template/static/fonts/demo.html  
  inflating: cv-template/static/fonts/iconfont.css  
  inflating: cv-template/static/fonts/iconfont.eot  
  inflating: cv-template/static/fonts/iconfont.svg  
  inflating: cv-template/static/fonts/iconfont.ttf  
  inflating: cv-template/static/fonts/iconfont.woff  
   creating: cv-template/static/image/
  inflating: cv-template/static/image/.DS_Store  
   creating: __MACOSX/cv-template/static/image/
  inflating: __MACOSX/cv-template/static/image/._.DS_Store  
  inflating: cv-template/static/image/bg.jpg  
  inflating: cv-template/static/image/weixin.png  
   creating: cv-template/static/js/
  inflating: cv-template/static/js/.DS_Store  
   creating: __MACOSX/cv-template/static/js/
  inflating: __MACOSX/cv-template/static/js/._.DS_Store  
  inflating: cv-template/static/js/modal.js  
  inflating: cv-template/static/js/script.js  
[root@jdu4e00u53f7 CV]# mv cv-template/* .
[root@jdu4e00u53f7 CV]# rm -rf cv-template*
cv-template/     cv-template.zip  
[root@jdu4e00u53f7 CV]# rm -rf cv-template* __MACOSX*
[root@jdu4e00u53f7 CV]# firefox index.html
Error: GDK_BACKEND does not match available displays
[root@jdu4e00u53f7 CV]# ls
index.html  static
[root@jdu4e00u53f7 CV]# yum install Xvfb libXfont xorg-x11-fonts* #下载界面运行
Loaded plugins: fastestmirror
Setting up Install Process
Loading mirror speeds from cached hostfile
epel/metalink                                                                          | 6.2 kB     00:00     
 * epel: ftp.cuhk.edu.hk
base                                                                                   | 3.7 kB     00:00     
extras                                                                                 | 3.4 kB     00:00     
updates                                                                                | 3.4 kB     00:00     
Package xorg-x11-server-Xvfb-1.17.4-16.el6.centos.x86_64 already installed and latest version
Package libXfont-1.5.1-2.el6.x86_64 already installed and latest version
Package xorg-x11-fonts-Type1-7.2-11.el6.noarch already installed and latest version
Resolving Dependencies
--> Running transaction check
---> Package xorg-x11-fonts-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-1-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-1-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-14-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-14-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-15-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-15-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-2-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-2-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-9-100dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ISO8859-9-75dpi.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-cyrillic.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-ethiopic.noarch 0:7.2-11.el6 will be installed
---> Package xorg-x11-fonts-misc.noarch 0:7.2-11.el6 will be installed
--> Finished Dependency Resolution
 
Dependencies Resolved
 
==============================================================================================================
 Package                                     Arch              Version                  Repository       Size
==============================================================================================================
Installing:
 xorg-x11-fonts-100dpi                       noarch            7.2-11.el6               base            3.1 M
 xorg-x11-fonts-75dpi                        noarch            7.2-11.el6               base            2.8 M
 xorg-x11-fonts-ISO8859-1-100dpi             noarch            7.2-11.el6               base            1.1 M
 xorg-x11-fonts-ISO8859-1-75dpi              noarch            7.2-11.el6               base            933 k
 xorg-x11-fonts-ISO8859-14-100dpi            noarch            7.2-11.el6               base            1.0 M
 xorg-x11-fonts-ISO8859-14-75dpi             noarch            7.2-11.el6               base            906 k
 xorg-x11-fonts-ISO8859-15-100dpi            noarch            7.2-11.el6               base            1.1 M
 xorg-x11-fonts-ISO8859-15-75dpi             noarch            7.2-11.el6               base            932 k
 xorg-x11-fonts-ISO8859-2-100dpi             noarch            7.2-11.el6               base            1.0 M
 xorg-x11-fonts-ISO8859-2-75dpi              noarch            7.2-11.el6               base            901 k
 xorg-x11-fonts-ISO8859-9-100dpi             noarch            7.2-11.el6               base            1.1 M
 xorg-x11-fonts-ISO8859-9-75dpi              noarch            7.2-11.el6               base            930 k
 xorg-x11-fonts-cyrillic                     noarch            7.2-11.el6               base            395 k
 xorg-x11-fonts-ethiopic                     noarch            7.2-11.el6               base            150 k
 xorg-x11-fonts-misc                         noarch            7.2-11.el6               base            5.8 M
 
Transaction Summary
==============================================================================================================
Install      15 Package(s)
 
Total download size: 22 M
Installed size: 23 M
Is this ok [y/N]: y
Downloading Packages:
(1/15): xorg-x11-fonts-100dpi-7.2-11.el6.noarch.rpm                                    | 3.1 MB     00:00     
(2/15): xorg-x11-fonts-75dpi-7.2-11.el6.noarch.rpm                                     | 2.8 MB     00:00     
(3/15): xorg-x11-fonts-ISO8859-1-100dpi-7.2-11.el6.noarch.rpm                          | 1.1 MB     00:00     
(4/15): xorg-x11-fonts-ISO8859-1-75dpi-7.2-11.el6.noarch.rpm                           | 933 kB     00:00     
(5/15): xorg-x11-fonts-ISO8859-14-100dpi-7.2-11.el6.noarch.rpm                         | 1.0 MB     00:00     
(6/15): xorg-x11-fonts-ISO8859-14-75dpi-7.2-11.el6.noarch.rpm                          | 906 kB     00:00     
(7/15): xorg-x11-fonts-ISO8859-15-100dpi-7.2-11.el6.noarch.rpm                         | 1.1 MB     00:00     
(8/15): xorg-x11-fonts-ISO8859-15-75dpi-7.2-11.el6.noarch.rpm                          | 932 kB     00:00     
(9/15): xorg-x11-fonts-ISO8859-2-100dpi-7.2-11.el6.noarch.rpm                          | 1.0 MB     00:00     
(10/15): xorg-x11-fonts-ISO8859-2-75dpi-7.2-11.el6.noarch.rpm                          | 901 kB     00:00     
(11/15): xorg-x11-fonts-ISO8859-9-100dpi-7.2-11.el6.noarch.rpm                         | 1.1 MB     00:00     
(12/15): xorg-x11-fonts-ISO8859-9-75dpi-7.2-11.el6.noarch.rpm                          | 930 kB     00:00     
(13/15): xorg-x11-fonts-cyrillic-7.2-11.el6.noarch.rpm                                 | 395 kB     00:00     
(14/15): xorg-x11-fonts-ethiopic-7.2-11.el6.noarch.rpm                                 | 150 kB     00:00     
(15/15): xorg-x11-fonts-misc-7.2-11.el6.noarch.rpm                                     | 5.8 MB     00:00     
--------------------------------------------------------------------------------------------------------------
Total                                                                          11 MB/s |  22 MB     00:01     
Running rpm_check_debug
Running Transaction Test
Transaction Test Succeeded
Running Transaction
  Installing : xorg-x11-fonts-ISO8859-9-100dpi-7.2-11.el6.noarch                                         1/15 
  Installing : xorg-x11-fonts-ISO8859-15-100dpi-7.2-11.el6.noarch                                        2/15 
  Installing : xorg-x11-fonts-ethiopic-7.2-11.el6.noarch                                                 3/15 
  Installing : xorg-x11-fonts-ISO8859-2-100dpi-7.2-11.el6.noarch                                         4/15 
  Installing : xorg-x11-fonts-ISO8859-15-75dpi-7.2-11.el6.noarch                                         5/15 
  Installing : xorg-x11-fonts-ISO8859-1-100dpi-7.2-11.el6.noarch                                         6/15 
  Installing : xorg-x11-fonts-cyrillic-7.2-11.el6.noarch                                                 7/15 
  Installing : xorg-x11-fonts-misc-7.2-11.el6.noarch                                                     8/15 
  Installing : xorg-x11-fonts-ISO8859-14-75dpi-7.2-11.el6.noarch                                         9/15 
  Installing : xorg-x11-fonts-ISO8859-2-75dpi-7.2-11.el6.noarch                                         10/15 
  Installing : xorg-x11-fonts-ISO8859-1-75dpi-7.2-11.el6.noarch                                         11/15 
  Installing : xorg-x11-fonts-75dpi-7.2-11.el6.noarch                                                   12/15 
  Installing : xorg-x11-fonts-ISO8859-14-100dpi-7.2-11.el6.noarch                                       13/15 
  Installing : xorg-x11-fonts-100dpi-7.2-11.el6.noarch                                                  14/15 
  Installing : xorg-x11-fonts-ISO8859-9-75dpi-7.2-11.el6.noarch                                         15/15 
  Verifying  : xorg-x11-fonts-ISO8859-9-75dpi-7.2-11.el6.noarch                                          1/15 
  Verifying  : xorg-x11-fonts-100dpi-7.2-11.el6.noarch                                                   2/15 
  Verifying  : xorg-x11-fonts-ISO8859-14-100dpi-7.2-11.el6.noarch                                        3/15 
  Verifying  : xorg-x11-fonts-75dpi-7.2-11.el6.noarch                                                    4/15 
  Verifying  : xorg-x11-fonts-ISO8859-1-75dpi-7.2-11.el6.noarch                                          5/15 
  Verifying  : xorg-x11-fonts-ISO8859-2-75dpi-7.2-11.el6.noarch                                          6/15 
  Verifying  : xorg-x11-fonts-ISO8859-14-75dpi-7.2-11.el6.noarch                                         7/15 
  Verifying  : xorg-x11-fonts-misc-7.2-11.el6.noarch                                                     8/15 
  Verifying  : xorg-x11-fonts-cyrillic-7.2-11.el6.noarch                                                 9/15 
  Verifying  : xorg-x11-fonts-ISO8859-1-100dpi-7.2-11.el6.noarch                                        10/15 
  Verifying  : xorg-x11-fonts-ISO8859-15-75dpi-7.2-11.el6.noarch                                        11/15 
  Verifying  : xorg-x11-fonts-ISO8859-2-100dpi-7.2-11.el6.noarch                                        12/15 
  Verifying  : xorg-x11-fonts-ethiopic-7.2-11.el6.noarch                                                13/15 
  Verifying  : xorg-x11-fonts-ISO8859-15-100dpi-7.2-11.el6.noarch                                       14/15 
  Verifying  : xorg-x11-fonts-ISO8859-9-100dpi-7.2-11.el6.noarch                                        15/15 
 
Installed:
  xorg-x11-fonts-100dpi.noarch 0:7.2-11.el6              xorg-x11-fonts-75dpi.noarch 0:7.2-11.el6             
  xorg-x11-fonts-ISO8859-1-100dpi.noarch 0:7.2-11.el6    xorg-x11-fonts-ISO8859-1-75dpi.noarch 0:7.2-11.el6   
  xorg-x11-fonts-ISO8859-14-100dpi.noarch 0:7.2-11.el6   xorg-x11-fonts-ISO8859-14-75dpi.noarch 0:7.2-11.el6  
  xorg-x11-fonts-ISO8859-15-100dpi.noarch 0:7.2-11.el6   xorg-x11-fonts-ISO8859-15-75dpi.noarch 0:7.2-11.el6  
  xorg-x11-fonts-ISO8859-2-100dpi.noarch 0:7.2-11.el6    xorg-x11-fonts-ISO8859-2-75dpi.noarch 0:7.2-11.el6   
  xorg-x11-fonts-ISO8859-9-100dpi.noarch 0:7.2-11.el6    xorg-x11-fonts-ISO8859-9-75dpi.noarch 0:7.2-11.el6   
  xorg-x11-fonts-cyrillic.noarch 0:7.2-11.el6            xorg-x11-fonts-ethiopic.noarch 0:7.2-11.el6          
  xorg-x11-fonts-misc.noarch 0:7.2-11.el6               
 
Complete
