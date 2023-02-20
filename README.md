### Install
1) Clone repo:
git clone https://github.com/ly552/zbxgrf01.git
2) Change owner grafana directory:
chown -R 472:472 grafana
3) Run docker-compose:
cd zabbix-docker
docker-compose up -d

### Debug
docker-compose logs --tail=1 -f
