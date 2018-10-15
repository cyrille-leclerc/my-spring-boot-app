pipeline {
    agent any
    stages {
        stage('Build and Deploy') {
            steps {
                withMaven() {
                    sh "./mvnw clean findbugs:findbugs deploy"
                }
            }
        }
    }
}
