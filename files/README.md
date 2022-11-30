# 安装
1、需要有java环境，安装default-jdk default-jdk-headless default-jre default-jre-headless。

2、wget https://raw.githubusercontent.com/GoussCN/pi-dc1-server/main/files/pi-dc1-server.sh

3、sudo bash pi-dc1-server.sh

 
# 卸载
1、wget https://raw.githubusercontent.com/GoussCN/pi-dc1-server/main/files/pi-dc1-server.sh

2、sudo bash pi-dc1-server.sh uninstall

# 命令
查看状态 systemctl status dc1server.service

启动服务 systemctl start dc1server.service

停止服务 systemctl stop dc1server.service


# 其他 
数据库文件位置/opt/dc1_database.db  
token配置文件/opt/dc1.conf，token=dc1server  
8000是dc1的数据端口  
8800是手机端的推送端口  
8880是手机端的http端口  
在浏览器中打开以下网址：http://ip:8880/api/queryDeviceList?token=111  
如果显示结果如下，说明服务端已经启动{"code": 403,"message": "token验证失败！"}  
