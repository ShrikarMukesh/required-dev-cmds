#disable jenkins from starting up automatically on start up <br/> 
update-rc.d jenkins disable 5

#enable to jenkins run from start up automatically <br/>
update-rc.d jenkins disable 5

#disable docker from running <br/>
sudo update-rc.d docker disable 5

sudo systemctl stop jenkins
sudo systemctl stop rabbitmq-server

***Docker process: <br/>

sudo systemctl status docker <br/>
sudo systemctl stop docker <br/>

docker update --restart=no $(docker ps -a -q) <br/>

$ sudo systemctl disable docker.service <br/>
$ sudo systemctl disable jenkins.service <br/>
$ sudo systemctl disable docker.socket <br/>


*****Jenkins process********** <br/>

sudo service jenkins start/stop/restart <br/>

sudo systemctl disable jenkins.service <br/>
sudo systemctl enable jenkins.service <br/>

*****Mongo DB***********
sudo systemctl status mongod <br/>
sudo systemctl start mongod <br/>
