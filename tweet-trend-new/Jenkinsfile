pipeline {
    agent {
        node {
            label 'maven'
        }
    }
environment {
    PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
}
    stages {
        stage('build') {
            steps {
                //dir('tweet-trend-new') {  // Schimbă în directorul care conține pom.xml
                sh 'mvn clean deploy'
                }
            }
        }
    }
}