
mmdvm屏幕固件中文通讯录（数据不是实时的，定期更新吧）     
pi-star版本：Pi-Star_RPi_V3.4.17    
热点版：双工，固件1.6     
屏幕固件版本：BD3OYD  
屏幕参数：3.5英寸 TJC4832T035_011  
数据来源：自由通dmr群  
数据格式：![1746973665382](https://github.com/user-attachments/assets/49c49459-8cc8-4fad-9ac2-38af8e6ad45b)  
安装教程 ：  
1.ssh登录树莓，ip：x.x.x.x,端口:22，默认用户名：pi-star，默认账号：raspberry  
2.1 rpi-rw; cd /tmp; sudo git clone https://github.com/ytsqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped.csv /usr/local/etc  
2.2 rpi-rw; cd /tmp; sudo git clone https://gitee.com/ytqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped.csv /usr/local/etc  
3.后台配置 nextion通讯录为stripped.csv：NextionDriver-DMRidFile：stripped.csv，配置地址DMRidFileSrc设置为https://github.com/ytsqkl/mmdvm-CNcontact/raw/main/stripped.csv或者https://gitee.com/ytqkl/mmdvm-CNcontact/raw/main/stripped.csv  
4.重启机器sudo reboot  
数据制作：中国（含港澳台地区），新加坡，马拉西亚，姓名合并到FIRST_NAME，国家和省份要甄别修改，不要出现问题，名字长的用简称要不显示不全。    
效果图：![1dbf7fb454de5432deb7a5c530e8e1d](https://github.com/user-attachments/assets/48aa2fdb-2fa3-411f-a5c1-76aed683021b)  

注意：如因mmdvm系统版本、屏幕驱动、屏幕固件等有差异，可能出现数据字段显示不准问题，请卸载屏幕驱动并重新安装，方法如下：  
rpi-rw
sudo rm -rf /usr/local/bin/NextionDriver
sudo rm -rf /etc/mmdvmhost.old
cd /tmp
sudo git clone https://gitee.com/BD3OYD/NextionDriverInstaller.git
sudo NextionDriverInstaller/install.sh   
感谢BD3OYD指导！！
