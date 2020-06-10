# webmin
## 免费VPS面板
## debian10

#常用软件包

apt-get -y update && apt-get -y install unzip zip wget curl mc nano sudo ufw socat gcc git cron gnupg


#安装 apt-key

wget -q http://www.webmin.com/jcameron-key.asc -O- | sudo apt-key add -


#添加源add the repository in your sources.list.d directory

echo "deb https://download.webmin.com/download/repository sarge contrib" | sudo tee /etc/apt/sources.list.d/webmin.list


#安装install

sudo apt update && sudo apt install -y webmin
