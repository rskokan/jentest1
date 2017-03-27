pipeline {

    agent any

    stages {
        stage('hello') {
            steps {
                echo "Hello!"
            }
        }

        stage('build') {
            steps {
                bat "gradlew clean build"
            }
        }
    }

    post {
        success {
            echo "We are done, build SUCCESS!"
        }
        failure {
            echo "Pipeline FAILED"
        }
    }


}
