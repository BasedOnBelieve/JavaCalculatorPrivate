pipeline {
    agent { label 'build-agent'}
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
