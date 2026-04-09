pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t mywebsite .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 80:80 mywebsite'
            }
        }
    }
}
