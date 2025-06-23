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
            }
        }
        stage('test') {
            steps {
                echo 'testing the application!'
            }
        }
        stage('deploy') {
            steps {
                echo 'deploying the application!'
            }
        }
    }
}
