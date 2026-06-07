pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'docker build -t my-web ./frontend'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker run -d -p 8000:80 my-web'
            }
        }
    }
}
