pipeline {
    agent any

    triggers {
        pollSCM '* * * * *'
    }
    stages {
        stage('Build') {
            steps {
                bat './gradlew assemble'
            }
        }
        stage('Test') {
            steps {
                bat './gradlew test'
            }
        }
    }
}
