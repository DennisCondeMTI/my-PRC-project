pipeline {
    agent any
    stages {
        stage('PRC') {
            steps {
                echo 'Laboratorio 04 - CI/CD Basics with Jenkins'
            }
        }
        stage('Build') {
            steps {
                bat 'docker run -p 8000:80 my-python-app'
            }
        }
    }

    post {
        success {
            echo 'Build completed succesfully!'
        }
        failure{
            echo 'Build failed'
        }
    }
}
