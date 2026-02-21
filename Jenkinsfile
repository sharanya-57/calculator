pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/sharanya-57/calculator.git'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac Calculator.java'
            }
        }

        stage('Build') {
            steps {
                sh 'java Calculator 25 5'
            }
        }

        stage('Test') {
            steps {
                sh 'java Calculator 30 5'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Completed'
            }
        }
    }
}
