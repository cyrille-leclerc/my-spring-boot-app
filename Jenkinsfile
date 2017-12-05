pipeline {
    agent any
    stages {
        stage('Build and Deploy') {
            steps {
                withMaven(maven: "maven-3.5",
                    mavenSettingsConfig: 'maven-settings-for-my-spring-boot-app') {
                    sh "mvn clean deploy"
                }
            }
        }
    }
}