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
                mvn clean install
            }
        }
        stage('Test') {
            steps {
                mvn clean test
            }
        }
        stage('Deploy') {
            steps {
                mvn clean deploy
            }
        }
    }
}
