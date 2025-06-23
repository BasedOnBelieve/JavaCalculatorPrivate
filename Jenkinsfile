pipeline {
    agent { label 'build-agent'}
    stages {
        stage('build') {
            steps {
                echo 'building the application!'
            }
        }
        stage('test') {
            when {
                expression {
                    BRANCH_NAME == 'test'
                }
            }
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
