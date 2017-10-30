# Installation step-by-step

\#Pre-req Java 8 ,utilities Installation

sudo yum install java-1.8.0-openjdk -y

sudo yum install unzip -y

sudo yum install wget





sudo mkdir /sonar

sudo chown ec2-user -R /sonar

cd /sonar

sudo wget[https://sonarsource.bintray.com/Distribution/sonarqube/sonarqube-6.0.zip](https://sonarsource.bintray.com/Distribution/sonarqube/sonarqube-6.0.zip)

sudo unzip sonarqube-6.0.zip

mv sonarqube-6.0 sonarqube

sudo ln -s /sonar/sonarqube/bin/linux-x86-64/sonar.sh /usr/bin/sonar

sudo chown ec2-user -R /sonar

sonar start

\#Access the sonar page on http://\(ec2hostname\):9999

sonar stop



