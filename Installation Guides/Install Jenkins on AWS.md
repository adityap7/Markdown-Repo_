# Install Jenkins on AWS

![github_jenkins width-2](https://github.com/adityap7/Markdown-Repo_/assets/6860928/24e8a264-8205-4a2c-b183-9750115cf3e1)

## About this tutorial
Jenkins: It is an open source automation server that manages the phases of software development. It includes building, testing, and deploying an application by facilitating continuous integration and continuous delivery. Jenkins is a server-based system that runs in servlet containers of Apache Tomcat.

Aws-Amazon Web Services,is a subsidiary of Amazon that provides on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered, pay-as-you-go basis. Clients will often use this in combination with autoscaling

## Steps for Installation:
Step - 1 Install Java
  - You need to Update your system-Use following command:
  
  ```
  sudo apt update
  ```
  - Now Install java-Use following command:
  ```
  sudo apt install openjdk-11-jre
  ```
  - To Validate Installation-Use following command:
  ```
  java -version
  ```
  It have to appearance some thing like this.
  ```
  openjdk version "11.0.12" 2021-07-20 OpenJDK Runtime Environment (build 11.0.12+7-post-Debian-2) OpenJDK 64-Bit Server VM (build          11.0.12+7-post-Debian-2, mixed mode, sharing)
  ```
Step - 2 Install Jenkins
  - Simply copy those commands and paste them onto your terminal:
  ```
  curl -fsSL https://pkg.jenkins.io/debian/jenkins.io.key | sudo tee \   /usr/share/keyrings/jenkins-keyring.asc > /dev/null
  ```
  ```
  echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \   https://pkg.jenkins.io/debian binary/ | sudo tee \                       /etc/apt/sources.list.d/jenkins.list > /dev/null
  ```
  ```
  sudo apt-get update
  ```
  ```
  sudo apt-get install jenkins
  ```
Step -3 Start jenkins
  - You need to use following commands:
  ```
  sudo systemctl enable jenkins
  ```
  ```
  sudo systemctl start jenkins
  ```
  ```
  sudo systemctl status jenkins
  ```
Step - 4 Open port 8080 from AWS Console

- In this way we have completed our installation of Jenkins on AWS.




  
