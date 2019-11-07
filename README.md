# Microservices

Microservices Materials

## White Papers

* [Fallacies of Distributed Computing Explained](./wp/wp-08fallacies-distributedcomputing.pdf)

   Source : Cirrus Minor Papers

   <https://arnon.me/presentations-papers-articles/>

   <http://www.rgoarchitects.com/Files/fallacies.pdf>


## Instructions

* [Getting started with the OCI Command Line Interface (CLI)](https://oracle.github.io/learning-library/oci-library/DevOps/OCI_CLI/OCI_CLI_HOL.html)

* Generate SSH Key 

   $ ssh-keygen -t rsa -N "" -b 2048 -C "<key_name>" -f <path/root_name>

* [user API key](https://docs.cloud.oracle.com/iaas/Content/API/Concepts/apisigningkey.htm#How)

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

   $  curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl

   $ chmod +x ./kubectl

   $ sudo mv ./kubectl /usr/local/bin/kubectl

   $ kubectl version

* Generate the Project

   $ mvn archetype:generate -DinteractiveMode=false \
    -DarchetypeGroupId=io.helidon.archetypes \
    -DarchetypeArtifactId=helidon-quickstart-se \
    -DarchetypeVersion=1.3.1 \
    -DgroupId=io.helidon.examples \
    -DartifactId=helidon-quickstart-se \
    -Dpackage=io.helidon.examples.quickstart.se



* Push Image to OCIR

   $ docker login iad.ocir.io

   > user: (Object Storage Namespace from Tenancy)/oracleidentitycloudservice/(username)

   > pass: Oauth Token

   $ docker tag helidon-quickstart-se:latest iad.ocir.io/(Object Storage Namespace from Tenancy)/repo1/helidon-quickstart-se:latest

   $ docker push iad.ocir.io/(Object Storage Namespace from Tenancy)/repo1/helidon-quickstart-se:latest


* [Mushop - Quickstart](https://github.com/oracle-quickstart/oci-cloudnative)
