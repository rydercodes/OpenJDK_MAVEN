# JAVA and MAVEN
Install OpenJDK 17 and Maven on Ubuntu 23

Before starting, you have to make sure that all Ubuntu OS packages installed on the server are up to date. You can do this by running the following commands:
```ruby
sudo apt update -y
sudo apt upgrade -y
```
Ubuntu’s default repository included Java 17. This is the easiest way to install the JDK using the apt package manager:
```ruby
sudo apt install openjdk-17-jdk
sudo apt install openjdk-17-jre
```
