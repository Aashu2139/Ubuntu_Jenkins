# Ubuntu_Jenkins

# link -- https://medium.com/@mosheezderman/how-to-set-up-ci-cd-pipeline-for-a-node-js-app-with-jenkins-c51581cc783c

# install on ubuntu -- https://www.jenkins.io/doc/book/installing/linux/#debianubuntu

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
JENKINS is written in JAVA so your system must have java / jdk (java development kit ) install on server as below
1 # sudo apt update
2 # sudo apt install openjdk-11-jre
3 # java --version 
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
now JENKINS installation on system
1 # curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
2 # echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
3 # sudo apt-get update
4 # sudo apt-get install jenkins
5 # jenkins --version 
6 jenkins installed succesfully 
7 # sudo systemctl enable jenkins && systemctl start jenkins (asks for password)
  # systemctl status jenkins.service (active running / shows your password for jenkins log in now paste your ip in tab )
8 **add port 8080** to run your jenkin on server 
  
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
YOU CAN DIRECTLY INSTALL DOCKER AND CREATE CONTAINER OF JENKINS IMAGE 
------------------------------------------------------------------------------------------------------------------------------------------------------------------------
now create one project on JENKINS AND repository on GIT-HUB and add webhook to get your repo connect with jenkins project


 
