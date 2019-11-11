### 1. Remove default old java
sudo yum -y remove java

### 2. Install at least java 1.8
sudo yum -y install java-1.8.0-openjdk

### 3. Download and install jenkins
sudo wget -O /etc/yum.repos.d/jenkins.repo http://pkg.jenkins-ci.org/redhat-stable/jenkins.repo
sudo rpm --import https://jenkins-ci.org/redhat/jenkins-ci.org.key
sudo yum -y install jenkins-2.164.2

### 4. Enable and run jenkins as a service
sudo systemctl enable jenkins
sudo systemctl start jenkins
