# docker-shadowsocks-libev

Fast build Docker Shadowsocks

Install Docker

# Sample: Centos7

yum -y install https://dl.fedoraproject.org/pub/epel/7/x86_64/e/epel-release-7-8.noarch.rpm

yum -y update

yum -y install docker-io

yum -y install python-pip

curl -L https://github.com/docker/compose/releases/download/1.8.1/docker-compose-`uname -s`-`uname -m` > /usr/local/bin/docker-compose

chmod +x /usr/local/bin/docker-compose

pip install -U docker-compose

systemctl enable supervisord

systemctl start docker

service docker restart

#
git clone https://github.com/tone497/docker-shadowsocks-libev.git

cd docker-shadowsocks-libev

./run.sh

open iptables 9453 port

aes-256-cfb

password:9453
