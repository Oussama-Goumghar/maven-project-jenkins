pipeline {
    agent any
    stages {
        stage ('maven install') {
            steps {
                withMaven (maven: 'maven3') {
                    sh 'mvn -f java-tomcat-sample/pom.xml clean install'
                }
            }
        }
    }   
}