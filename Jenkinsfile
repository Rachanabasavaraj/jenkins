pipeline {
    agent {
        docker {
            image 'node:16-alpine'
            args '-v /tmp:/tmp'
        }
    }
    stages {
        stage('Test Docker Slave') {
            steps {
                sh 'echo "Docker slave is working!"'
                sh 'node --version'
                sh 'whoami'
                sh 'hostname'
            }
        }
    }
}
