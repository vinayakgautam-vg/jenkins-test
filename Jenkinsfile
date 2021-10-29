pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..' 
                  
                   bash '#!/bin/bash sudo docker build -t myimage . '
                   
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
  
