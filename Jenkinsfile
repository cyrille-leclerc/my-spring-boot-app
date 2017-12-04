pipeline {
    agent {
        docker {
            image "maven:3-jdk-8"
        }
    }
    stages {
        stage('Build and Deploy') {
            steps {
                withMaven(
                    mavenSettingsConfig: 'maven-settings-for-my-spring-boot-app') {

                    sh "mvn clean deploy"
                }
            }
        }
    }
}