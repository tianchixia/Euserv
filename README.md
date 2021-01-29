# Euserv
Euserv一键安装教程
首选需要一个EUserv的免费实例，怎么注册油管上有很多教程，我这里就不多说了。
用SSH登录后
第一步输入
echo -e "nameserver 2001:67c:2b0::4\nnameserver 2001:67c:2b0::6" > /etc/resolv.conf
第二步安装wget、curl
Centos
yum update && yum install -y wget curl
Debian
apt update && apt install wget curl -y
Ubuntu
apt-get update && apt-get install wget -y
第二步输入mack a 的一键脚本
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
安装过程有中文说明，很容易
智能解析DNS服务，我选择N
安装成功复制一下代码就OK了
