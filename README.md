# Microservices

Microservices Materials

## White Papers

* [Fallacies of Distributed Computing Explained](./wp/wp-08fallacies-distributedcomputing.pdf)

   Source : Cirrus Minor Papers

   <https://arnon.me/presentations-papers-articles/>

   <http://www.rgoarchitects.com/Files/fallacies.pdf>


## Instructions

* Install Java

   $ sudo yum -y install java

* Install Maven

   $ sudo yum -y install maven

* Install Docker

   $ sudo yum install -y docker-engine

   $ sudo systemctl enable docker

   $ sudo systemctl start docker

   $ sudo systemctl status docker.service

* Install kubectl

   $  curl -LO https://storage.googleapis.com/kubernetes-release/release/\`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt\`/bin/linux/amd64/kubectl

   $ chmod +x ./kubectl

   $ sudo mv ./kubectl /usr/local/bin/kubectl

   $ kubectl version




