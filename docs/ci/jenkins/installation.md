---
title: Jenkins Installation
parent: Jenkins CI
grand_parent: Continuous Integration
nav_order: 1
---


# **Installation and Configuration References**

https://wiki.jenkins.io/display/JENKINS/Installing+Jenkins+on+Red+Hat+distributions





# Installation Commands step-by-step



\# Pre-req Java 8 , utilities Installation

sudo yum install java-1.8.0-openjdk -y

sudo yum install java-devel

sudo yum install wget



\# Jenkins package installation

sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat/jenkins.repo

sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key

sudo yum install jenkins



sudo service jenkins start

sudo chkconfig jenkins on



Access your Jenkins

http://&lt;&lt;ec2-instance\_public\_dns&gt;&gt;:8080

ex: [http://ec2-54-84-83-156.compute-1.amazonaws.com:8080](http://ec2-54-84-83-156.compute-1.amazonaws.com:8080)





![](file:///C:/Users/SAIRAM~1/AppData/Local/Temp/msohtmlclip1/01/clip_image002.jpg)



ssh to you ec2 instance and get the intial password:-

sudo cat /var/lib/jenkins/secrets/initialAdminPassword





Install Suggested Plugins

Fill out **all** the details and create an admin user



