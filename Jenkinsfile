pipeline {
    stages {
        // Get the actual docker images sourcse from oracle git account
        stage('Get Sources') {
            steps {
                git url: 'https://github.com/oracle/docker-images.git'
            }
        }
        stage('Build Oracle Docker Images') {
            steps {
                // build the image
                sh 'sudo ./buildDockerImage.sh  -v 12.2.0.1.0
            }
        }
    }
}   
