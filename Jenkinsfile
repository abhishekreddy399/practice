pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'docker build -t abhi754/my-web:v1 ./frontend'
            }
        }

        stage('Login') {
            steps {
                bat 'docker login -u abhi754 -p dckr_pat_vpbG9rS9KPm1aoL98do-_B1uRfs'
            }
        }

        stage('Push') {
            steps {
                bat 'docker push abhi754/my-web:v1'
            }
        }
    }
}
