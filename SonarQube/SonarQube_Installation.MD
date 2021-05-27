# SonarQube Installation

SonarQube provides the capability to not only show health of an application but also to highlight issues newly introduced. With a Quality Gate in place, you can fix the leak and therefore improve code quality systematically.

### Prerequisites
1. EC2 instance with Java installed


### Installation

Download stable SonarQube version from below website. 
- Website: https://www.sonarqube.org/downloads/

Download & unzip SonarQube 6.0
```sh
# cd /opt
# wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-6.7.7.zip
# unzip sonarqube-6.7.7.zip
# mv /opt/sonarqube-6.7.7 /opt/sonar
```


Start SonarQube service 
```sh
# cd /opt/sonar/bin/linux-x86-64/
# ./sonar.sh start
```


Start SonarQube server
```sh
# service sonar start
```
SonarQube application uses port 9000. access SonarQube from browser
```sh
  http://<EC2_PUBLIC_IP>:9000/sonar
```
###  Troubleshooting 

1. Check whether you enabled port 9000 in EC2 instance security group


