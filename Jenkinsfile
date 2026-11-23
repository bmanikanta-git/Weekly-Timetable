pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                echo 'Building'
                bat 'text -f index.html'
            }
        }
        stage('Test'){
            steps{
                bat 'grep -q Weekly Time Table index.html'
            }
        }
    }
}