*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
*********************************请根据版本选择否则会出现屏幕字段不准确现象。*************************************************   
版本一、mmdvm屏幕固件中文通讯录 
pi-star版本：Pi-Star_RPi_V4.2.3_18 
热点版：双工，固件1.5  
屏幕固件版本：BD3OYD  
屏幕参数：3.5英寸 TJC4832T035_011  
数据来源：自由通dmr群  
数据格式：![1746973665382](https://github.com/user-attachments/assets/49c49459-8cc8-4fad-9ac2-38af8e6ad45b)
安装教程 ：  

1.ssh登录树莓，ip：x.x.x.x,端口:22，默认用户名：pi-star，默认账号：raspberry  
2.1 rpi-rw; cd /tmp; sudo git clone https://github.com/ytsqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped.csv /usr/local/etc  
2.2 rpi-rw; cd /tmp; sudo git clone https://gitee.com/ytqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped.csv /usr/local/etc  
3.后台配置 nextion通讯录为stripped.csv：NextionDriver-DMRidFile：stripped.csv，配置地址：DMRidFileSrc-https://gitee.com/ytqkl/mmdvm-CNcontact/raw/main/stripped.csv  
4.重启机器sudo reboot  
数据制作：中国（含港台地区），新加坡，马拉西亚，姓名合并到FIRST_NAME，国家和省份要甄别修改，名字长的用简称要不显示不全。
版本二、mmdvm屏幕固件中文通讯录 
pi-star版本：Pi-Star_RPi_V3.4.17
热点版：双工，固件1.6
屏幕固件版本：BD3OYD  
屏幕参数：3.5英寸 TJC4832T035_011  
数据来源：自由通dmr群  
数据格式：
![1746973809106](https://github.com/user-attachments/assets/f151b376-0365-4b5c-80cb-0c1e6b607953)

安装教程 ：  
1.ssh登录树莓，ip：x.x.x.x,端口:22，默认用户名：pi-star，默认账号：raspberry  
2.1 rpi-rw; cd /tmp; sudo git clone https://github.com/ytsqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped-3.4.17.csv /usr/local/etc/stripped.csv   
2.2 rpi-rw; cd /tmp; sudo git clone https://gitee.com/ytqkl/mmdvm-CNcontact.git; cd /tmp/mmdvm-CNcontact; sudo cp stripped-3.4.17.csv /usr/local/etc/stripped.csv  
3.后台配置 nextion通讯录为stripped.csv：NextionDriver-DMRidFile：stripped.csv，配置地址：DMRidFileSrc-https://gitee.com/ytqkl/mmdvm-CNcontact/raw/main/stripped.csv   
4.重启机器sudo reboot  
数据制作：中国（含港台地区），新加坡，马拉西亚，姓名合并到FIRST_NAME，国家和省份要甄别修改，名字长的用简称要不显示不全。
