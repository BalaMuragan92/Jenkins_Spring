pipeline {
    agent any

    stages {
    	stage('Clone') {
            steps {
                echo 'Cloning..'
                git url: 'https://github.com/kaushik12499/Jenkins_Spring.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh mvn clean install
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh mvn clean test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh mvn clean deploy
            }
        }
    }
}
