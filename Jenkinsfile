pipeline {
    agent any
    tools {
        maven 'maven3'
        jdk 'java8'
    }
    stages {
        stage('init') {
            steps {
                echo "This is initializing stage"
            }
        }

        stage('Build') {
            steps {
                echo "This is Build Stage"
                sh label: '', script: 'mvn clean package checkstyle:checkstyle'
            }
        }

        stage('Deploy') {
            steps {
                echo "This is Deployment Stage"
            }
        }
    }
}