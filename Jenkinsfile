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
                    maven: 'M3',
                    mavenSettingsConfig: 'maven-settings-for-my-spring-boot-app') {

                    sh "mvn clean deploy"
                }
            }
        }
    }
}