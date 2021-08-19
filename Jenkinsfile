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
                mvn clean install
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                mvn clean test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                mvn clean deploy
            }
        }
    }
}
