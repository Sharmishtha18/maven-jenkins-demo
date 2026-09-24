pipeline {
    agent any

    tools {
        maven 'maven-cicd'
    }

    stages {
        stage('Checkout') {
            steps {
               checkout scm
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Result') {
            steps {
                echo 'Maven build completed.'
            }
        }
    }
}
