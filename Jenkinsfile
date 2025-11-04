pipeline {
    agent any

    tools {
        jdk 'java-17'
        maven 'maven-3.8'
    }

    stages {
        stage('git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/Siva123569/Boardgamejenkins.git'
            }
        }

        stage('maven compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('maven package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
