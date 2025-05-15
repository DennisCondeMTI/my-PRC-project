pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('build') {
            steps {
                powershell 'dir'
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
