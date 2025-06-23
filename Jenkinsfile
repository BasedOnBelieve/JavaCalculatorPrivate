pipeline {
    agent { label 'build-agent'}
    tools {
        maven 'maven'
    }
    stages {
        stage('veryfying maven') {
            steps { sh 'mvn -version'
            }
        }
        stage('build') {
            steps {
                echo 'building the application!'
                sh 'mvn package'
            }
        }
        stage('test') {
            steps {
                echo 'testing the application!'
                sh 'java -jar target/*.jar 10 20'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploying the application!'
            }
        }
    }
}
