se lab



1)Jenkins

-> 2stage pipeline

-> 3stage pipeline



-> ngrok -login

   paste auth key in ngrok cmd, paste .exe http 8888

   past the forwarding url in GitHub with https://chemurgic-unpoignantly-joel.ngrok-free.dev/github-webhook/

   makes changes in git before that build the project



-> email (plugin - email extension)

   email notification - smtp.gmail.com , mail , appkey, ssl , 465, mail

   extended email - smtp.gmail.com , 465 , mail and appkey , ssl , triggers

   editable emial - just provide mail at receipant list







-> script pipeline

**pipeline {**

    **agent any**

    **tools{**

        **maven 'MAVEN-HOME'**

    **}**

    **stages {**

        **stage('git repo \& clean') {**

            **steps {**

                **//bat "rmdir  /s /q mavenjava"**

                **bat "git clone provide your github link"**

                **bat "mvn clean -f mavenjava"**

            **}**

        **}**

        **stage('install') {**

            **steps {**

                **bat "mvn install -f mavenjava" #project name#**

            **}**

        **}**

        **stage('test') {**

            **steps {**

                **bat "mvn test -f mavenjava"**

            **}**

        **}**

        **stage('package') {**

            **steps {**

                **bat "mvn package -f mavenjava"**

            **}**

        **}**

    **}**

**}**







2)minikube

-> mkdir se

-> cd se

-> docker login

-> docker pull hubimage

-> minikube start --driver=docker

-> minikube status

-> kubectl get pods

-> kubectl get deployments

-> kubectl create deployment imagename --image=hubname

-> kubectl get pods

-> kubectl get deployments

-> kubectl scale deployment imagename --replicas=no

-> kubectl expose deployment imagename --type=NodePort --port=8080

-> kubectl get svc

-> kubectl port-forward svc/imagename 7777:8080

-> kubectl delete deployment name







3)nagios

-> docker login

-> docker pull jasonriver/nagois:latest

-> docker run -p 7070:80 --name nagiosdemo jasonrivers/nagios:latest

-> docker rm container

-> docker rmi image





4)aws

-> aws untitled

-> aws courses

-> aws modules , start lab

-> Ec2 service , launch instance

-> select name , ubuntu ,everything go by default

-> create a pem file

-> allow https and http , select edit and alltraffic anywhere

-> click launch instance

-> connect and copy ssh key

-> open PowerShell goto downloads paste sshkey

-> check docker verion git , sudo su, sudo apt-get update , sudo apt-get install docker.io

-> mkdir , git clone the url , build the image

-> run the image

-> copy and run the ip address in chrome





5)uml

-> usecase

-> class

-> sequence 

-> component

