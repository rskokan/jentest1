#!groovy

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                gradlew build
            }
        }
        stage('Test'){
            steps {
                echo 'Testing...'
                // sh 'make check'
                // junit 'reports/**/*.xml'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // sh 'make publish'
            }
        }
    }
}
