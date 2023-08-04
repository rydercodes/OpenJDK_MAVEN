# JAVA and MAVEN
Install Java OpenJDK 17 and Maven on Ubuntu 23

### OpenJDK
Before starting, you have to make sure that all Ubuntu OS packages installed on the server are up to date. You can do this by running the following commands:
```
sudo apt update -y
sudo apt upgrade -y
```
Ubuntu’s default repository included Java 17. This is the easiest way to install the JDK using the apt package manager:
```
sudo apt install openjdk-17-jdk
sudo apt install openjdk-17-jre
```
now you can check the version of Java:
```
java --version
```
in case it doesn't shows the version. you should add the home directory and bin directory of Java in the PATH of the system.
run the following:
if the nano is not installed:
```
sudo apt install nano
```
by default Java installed in the `/usr/lib/jvm/` directory. in my case it is in the following directory:
` /usr/lib/jvm/java-17-openjdk-amd64`

```
cd nano ~/.bashrc
```
in the last line add the following:
```
export PATH=$PATH:/usr/lib/jvm/java-17-openjdk-amd64
export PATH=$PATH:/usr/lib/jvm/java-17-openjdk-amd64/bin
```
then save and exit by using `Ctrl + O` for save and `Ctrl + X` for close bashrc. After you did, write `source ~/.bashrc` in the terminal to save permanently and re-session.

### Maven
Download the `Binary tar.gz archive` from [Apache Maven Download Center](https://maven.apache.org/download.cgi)
go to the downloaded directory and extract it by `sudo tar xzvf apache-maven-3.9.4-bin.tar.gz` and add the `bin` directory of the maven to the paths like java. 
after that by running `mvn --version`, you can see the maven version.
