pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'docker build -t abhi754/my-web:v1 ./frontend'
            }
        }

        stage('Deploy') {
            steps {
                bat 'docker push abhi754/myweb:v1'
            }
        }
    }
}
