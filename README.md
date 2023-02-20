### Install git & docker & docker-compose
https://docs.docker.com/engine/install/ubuntu/

apt install git docker-compose 

### Install zbxgrf01
1) Clone repo:
git clone https://github.com/ly552/zbxgrf01.git
2) Change owner grafana directory:
cd zbxgrf01
chown -R 472:472 grafana
3) Run docker-compose:
cd zbxgrf01
docker-compose up -d

### Settings & ports
1)Zabbix :80, Admin:zabbix

2)Grafana :3000, admin:admin

Plugin:
HTTP URL: http://localhost-ip/api_jsonrpc.php
Zabbix API details User: Admin
Zabbix API details Password: zabbix

### Debug
docker-compose logs --tail=1 -f
