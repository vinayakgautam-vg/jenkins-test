pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..' 
                   sh('apt update -y')
                   sh('apt install docker.io -y')
                   sh('docker build -t myimage . ')
                   
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh '#!/bin/bash'
                sh 'sudo docker run -it -d --name mycontainer -p 80:80 myimage'
           }
        }
    }
}
  
