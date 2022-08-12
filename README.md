# SysLog-Server-Easticsearch-Logstash-Grafana-Installation-Guide
Guide for the installation of a SysLog Server using ElasticSearch, Logstash and Grafana

sudo apt-get update

sudo apt-get upgrade

sudo apt-get install default-jdk -y

java -version

![image](https://user-images.githubusercontent.com/20743678/184070434-bc16f6f0-4988-41e1-950c-6a948c037ea9.png)

cd /tmp

mkdir elk

cd elk

wget https://artifacts.elastic.co/downloads/elasticsearch/elasticsearch-8.3.3-amd64.deb

![image](https://user-images.githubusercontent.com/20743678/184342967-923fef8b-8823-4705-bc64-ba3897e62fed.png)

dpkg -i elasticsearch-8.3.3-amd64.deb

![image](https://user-images.githubusercontent.com/20743678/184346009-ef368693-3aaa-40d1-9daf-5aada666105d.png)

systemctl status elasticsearch

systemctl enable elasticsearch

systemctl start elasticsearch

![image](https://user-images.githubusercontent.com/20743678/184346309-4cad6569-f916-43ab-b9cd-946e90c2293e.png)

cd /etc/elasticsearch

sudo nano elasticsearch.yml

![image](https://user-images.githubusercontent.com/20743678/184347029-c392cbe8-08f9-4748-afc7-401219292fae.png)

curl http://localhost:9200

![image](https://user-images.githubusercontent.com/20743678/184349689-c01d38e1-a766-44dc-9856-475d935d729d.png)

wget https://artifacts.elastic.co/downloads/kibana/kibana-8.3.3-amd64.deb

![image](https://user-images.githubusercontent.com/20743678/184352101-724c8ef0-6122-4be5-9bea-71f9c1823dd4.png)

sudo dpkg -i kibana-8.3.3-amd64.deb 

systemctl status kibana

systemctl enable kibana

systemctl start kibana

![image](https://user-images.githubusercontent.com/20743678/184352743-c2292d39-4934-42ee-a32e-1c0a6181b738.png)

sudo nano /etc/kibana/kibana.yml

![image](https://user-images.githubusercontent.com/20743678/184353068-1fdfc01d-b147-4055-a137-bee8e7a93912.png)
