pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'docker build -t my-web ./frontend'
            }
        }

        stage('Deploy') {
            steps {
                bat 'docker run -d -p 8000:80 my-web'
            }
        }
    }
}
