安装
-----------------------------
1、需要有java环境，安装default-jdk default-jdk-headless default-jre default-jre-headless。

2、wget https://raw.githubusercontent.com/GoussCN/pi-dc1-server/main/files/pi-dc1-server.sh

3、sudo bash pi-dc1-server.sh

 
卸载
-----------------------------
1、wget https://raw.githubusercontent.com/GoussCN/pi-dc1-server/main/files/pi-dc1-server.sh

2、sudo bash pi-dc1-server.sh uninstall

命令
-----------------------------
查看状态 systemctl status dc1server.service

启动服务 systemctl start dc1server.service

停止服务 systemctl stop dc1server.service
