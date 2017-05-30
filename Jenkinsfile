#!groovy

node {
    checkout scm
    stage('Build and Deploy') {
        withMaven(
            maven: 'M3', 
            mavenSettingsConfig: 'maven-settings-for-my-spring-boot-app') {
            sh "mvn clean deploy"
        }
    }
}