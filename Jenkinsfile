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
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                echo "TEST"
                sh 'mvn clean test'
            }
        }
        stage('Deploy') {
            steps {
                echo "DEPLOY"
                
            }
        }
    }
}
