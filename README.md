# netology-zabbix-hw

#2 Задание 1

https://github.com/netology-code/smon-homeworks/blob/main/hw-01-new.md


![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_280.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_281.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_282.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_283.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_285.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_286.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_287.png)


## Задание 2

https://github.com/netology-code/smon-homeworks/blob/main/hw-02.md


![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_290.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_291.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_292.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_293.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_294.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_295.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_296.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_297.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_298.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_299.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_300.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_301.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_302.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_303.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_304.png)

### Команды
sudo apt update && sudo apt upgrade -y

sudo apt install postgresql

sudo wget https://repo.zabbix.com/zabbix/7.0/debian/pool/main/z/zabbix-release/zabbix-release_latest_7.0+debian12_all.deb

sudo dpkg -i zabbix-release_latest_7.0+debian12_all.deb

sudo apt update

sudo apt install zabbix-server-pgsql zabbix-frontend-php php8.2-pgsql zabbix-apache-conf zabbix-sql-scripts zabbix-agent

sudo -u postgres createuser --pwprompt zabbix

sudo -u postgres createdb -O zabbix zabbix

sudo zcat /usr/share/zabbix-sql-scripts/postgresql/server.sql.gz | sudo -u zabbix psql zabbix 

sudo vim /etc/zabbix/zabbix_server.conf

sudo systemctl restart zabbix-server zabbix-agent apache2

sudo systemctl enable zabbix-server zabbix-agent apache2

-----хост 
sudo dnf install zabbix-agent
vim /etc/zabbix_agentd.conf  

-----windows
Через GUI


## Задание 3

Изначально для каждого сервера был свой шаблон, потом они были слиты и использовался только первый

так как команда для цпу бралась из шаблона linux by zabbix agent пришлось погуглилить и изменить на proc.cpu.util

Так же проверл тесты с загруской пасяти и цпу - на скриншотах.

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_506.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_507.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_508.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_509.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_510.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_511.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_512.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_513.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_514.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_515.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_516.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_517.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_518.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_519.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_520.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_521.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_522.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_523.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_524.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_525.png)

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_526.png)


На задании со сзвездой прям на первом не смог понять как прикрутить именно agent.ping, в списке его нет.
попробую сделать позже.

![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_527.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_528.png)
![alt text](https://github.com/SLzDevOps/netology-zabbix-hw/blob/main/Screenshot_529.png)






