# dockerPSIRSBackend
A compose DockerFile to run the PSIRS backend application

## Setup
* Drop these file and directory into the top level directory of the project
* Run  `docker-compose up`


## Note
* If you have local installations of Mysql and apache on your machines, make sure you put off the applications to free the ports.

* Apache exposes through port 8000
* Adminer, which is our database designer exposes through port 8082


## Extra Information

To clean up your images and containers:
* Run the three commands below:
*	 `docker stop $(docker ps -aq)`
*	 `docker rm $(docker ps -aq)`
*	 `docker rmi $(docker images -q)`

To have shell access to your container
* docker exec -it psirsbackend_web_1 bash -c "sudo -u devuser /bin/bash”


## Contributors
[Daser David](https://github.com/daser)
