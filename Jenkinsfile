pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building'
                bat 'type index.html'
            }
        }

        stage('Test') {
            steps {
                bat 'findstr /C:"Weekly Time Table" index.html'
                echo 'Test Successful'
            }
        }
    }
}
