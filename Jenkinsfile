pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'                 
            }
            steps { 
                sh 'docker -version'
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
  
