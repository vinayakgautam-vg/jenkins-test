pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..' 
                    
                   sh 'echo "building a container" ' 
                   sh 'sudo apt update -y' 
                   sh 'sudo apt install docker.io -y' 
                   sh 'sudo docker build -t myimage . '
                   
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
                sh 'sudo docker run -it -d --name mycontainer -p 80:80 myimage'
           }
        }
    }
}
  
