pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'                 
                sh 'sudo apt install docker.io -y'
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
             
           }
        }
    }
}
  
