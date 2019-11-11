### 1. Get gradle
wget -O ~/gradle-4.7-bin.zip https://services.gradle.org/distributions/gradle-4.7-bin.zip
### 2. Install Java
sudo yum -y install unzip java-1.8.0-openjdk
### 3. Unzip gradle zipfile into /opt/gradle
sudo mkdir /opt/gradle
sudo unzip -d /opt/gradle ~/gradle-4.7.bin.zip
### 4. Create gradle.sh file
sudo vi /etc/profile.d/gradle.sh
put this to gradle.sh file:
export PATH=$PATH:/opt/gradle/gradle-4.7/bin
### 5. Set permissions
sudo chmod 755 /etc/profile.d/gradle.sh
### 6. Check gradle installation
gradle --version
