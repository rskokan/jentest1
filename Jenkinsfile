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
                gradlew build
            }
        }
    }
}
