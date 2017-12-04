pipeline {
    agent {
        docker {
            image "openjdk:8-jdk"
        }
    }
    stages {
        stage('Build and Deploy') {
            steps {
                withMaven(
                    mavenSettingsConfig: 'maven-settings-for-my-spring-boot-app') {

                    sh "./mvnw clean deploy"
                }
            }
        }
    }
}