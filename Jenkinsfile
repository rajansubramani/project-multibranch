//Decalartive Pipeline

pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script{
                     sh 'npm install'
                }
            }
        }
        stage('Docker Build Images') {
            steps {
                script {
                    sh 'docker build -t rajansubramani/9thfeb:v2 .'
                    sh 'docker images'
                }
            }
        }
    }
}
