# Install and Configure Maven & git in Jenkins server

## Install Maven
```sh
yum install wget
wget https://dlcdn.apache.org/maven/maven-3/3.9.7/binaries/apache-maven-3.9.7-bin.tar.gz
tar -xvzf apache-maven-3.9.7-bin.tar.gz
export M2_HOME=/opt/apache-maven-3.9.7
export M2=$M2_HOME/bin
PATH=$PATH:$M2
# To set it permanently update your .bash_profile
source ~/.bash_profile

Validate Maven

mvn version
```

## Install git
```sh
yum install git


```

## Assign shell to jenkins user

```sh
vi /etc/passwd
change shell from /bin/false to /bin/bash
```

