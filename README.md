# SysLog-Server-Easticsearch-Logstash-Grafana-Installation-Guide
Guide for the installation of a SysLog Server using ElasticSearch, Logstash and Grafana

sudo apt-get update

sudo apt-get upgrade

sudo apt-get install default-jdk -y

java -version

![image](https://user-images.githubusercontent.com/20743678/184070434-bc16f6f0-4988-41e1-950c-6a948c037ea9.png)

sudo apt-get install apt-transport-https -y

![image](https://user-images.githubusercontent.com/20743678/184070495-86775951-ceb5-4326-adc9-a26feffe5249.png)

url -fsSL https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -

![image](https://user-images.githubusercontent.com/20743678/184070540-ebdebb25-e9ac-41ac-a627-c1ceac879003.png)

sudo apt-get install curl

![image](https://user-images.githubusercontent.com/20743678/184070611-4419ad0f-a9fc-4d6e-8688-ab44041fe184.png)

wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo gpg --dearmor -o /usr/share/keyrings/elasticsearch-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/elasticsearch-keyring.gpg] https://artifacts.elastic.co/packages/8.x/apt stable main" | sudo tee /etc/apt/sources.list.d/elastic-8.x.list

sudo apt update -y

sudo apt-get install elasticsearch -y

![image](https://user-images.githubusercontent.com/20743678/184070814-5fbfa251-e8dc-4460-89e0-ed7a28132b01.png)

