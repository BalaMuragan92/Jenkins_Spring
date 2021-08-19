pipeline {
    agent any

    stages {
    	stage('Clone') {
            steps {
                git url: 'https://github.com/kaushik12499/Jenkins_Spring.git'
            }
        }
        stage('Build') {
            steps {
                echo "BUILD"
            }
        }
        stage('Test') {
            steps {
                echo "TEST"
            }
        }
        stage('Deploy') {
            steps {
                echo "DEPLOY"
            }
        }
    }
}
