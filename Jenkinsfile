pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "building a container" 
                sudo apt update -y 
                sudo apt install docker.io -y 
                sudo docker build -t myimage .
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
                sudo docker run -it -d --name mycontainer -p 80:80 myimage 
           }
        }
    }
}
