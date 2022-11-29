# pi-dc1-server
树莓派架设DC1服务器

1、DNS劫持, /etc/dnsmasq.conf, /etc/hosts  
address=/phicomm.me/192.168.1.11  
address=/smartplugconnect.phicomm.com/192.168.1.11  
address=/p.to/192.168.1.11  
address=/aircat.phicomm.com/192.168.1.11  

192.168.1.11 phicomm.me  
192.168.1.11 smartplugconnect.phicomm.com  
192.168.1.11 p.to  
192.168.1.11 aircat.phicomm.com  

2、DC1智能插板WiFi指示灯及操作说明：  
  2.1、常亮，表示插线板已连接WiFi；  
  2.2、慢闪，表示插线板未连接WiFi；  
  2.3、快闪，表示插线板进入配网状态；  
  2.4、长按电源开关3秒，进入配网状态（WiFi指示灯快闪为5分钟，到时间自动解除配网状态）；  
  2.5、长按电源开关15秒以上，直至插线板断电重启，此时恢复出厂设置，WiFi指示灯为熄灭状态。  




























备注：所有代码源于网络，如有侵权请告知删除。
