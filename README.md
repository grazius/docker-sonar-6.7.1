# sonar-6.7.1
fork of official docker file for non root users launch  
  
docker build -t grazius-sonarqube .  
docker run -d -u 1001:1001 --name sonarqube -p 9000:9000 -p 9092:9092 -v /tmp/sonarqube/plugins:/sonar-plugins grazius-sonarqube  
docker rm sonarqube  

