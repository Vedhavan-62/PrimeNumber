pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/USERNAME/PrimeNumber.git'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac PrimeNumber.java'
            }
        }

        stage('Execute') {
            steps {
                sh 'echo 7 | java PrimeNumber'
            }
        }
    }
}
