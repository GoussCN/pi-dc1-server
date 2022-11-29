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

3、DC1配置入网（DC1连接wifi,且只支持2.4G）  
  3.1、接通DC1电源，长按电源开关3秒，此时WiFi指示灯快速闪烁，表示进入配网状态；  
  3.2、电脑的无线连接上DC1的WiFi（如PHI_PLUG1_XXXX）后，打开网络调试助手(NetAssist.exe)；  
    (1)、协议类型-选择UDP  
    (2)、本地主机地址-选择本机IP  
    (3)、本地主机端口-输入7550  
    (4)、点击打开按钮  
    (5)、打开按钮打开后，下方显示为“远程主机：192.168.4.1:7550”；  
    (6)、然后再数据发送输入框中输入如下代码：  
  
{"header":"phi-plug-0001","uuid":"00010","action":"wifi=","uuid":"identify291f","auth":"","params":{"ssid":"WiFi名","password":"WiFi密码"}}  

注意1，要修改成你自己WiFi的名字和密码，  
注意2，要在上述内容后打个回车，然后再按发送。然后应该会收到如下配网成功的信息。  



























备注：所有代码源于网络，如有侵权请告知删除。
