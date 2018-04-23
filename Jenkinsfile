#!groovy

node {
    checkout scm
    stage('Build and Deploy') {
        withMaven() {
            sh "mvn clean deploy"
        }
    }
}