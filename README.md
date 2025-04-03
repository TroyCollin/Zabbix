# Zabbix
Setup Zabbix with Docker

usage: 
docker compose up -d

To verify backups:
docker exec -it mysql-backup sh
ls /var/backups/mysql

To restore a backup:
docker exec -i mysql-server mysql -u zabbix -pzabbix_pwd zabbix < /path/to/backup.sql
