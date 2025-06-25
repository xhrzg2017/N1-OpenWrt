新建虛擬网段
docker network create --subnet=172.18.10.0/24 --gateway 172.18.10.1 MyNET
新建adg 172.18.10.2
docker run -d --name AdGuard-Home1 -v /opt/docker/AGH_Docker1:/opt/adguardhome/work -v /opt/docker/AGH_Docker1:/opt/adguardhome/conf -p 3001:3000 --restart always --net MyNET --ip 172.18.10.2 adguard/adguardhome:latest



openclash加自定义规则
- IP-CIDR,172.18.10.2/32,DIRECT
