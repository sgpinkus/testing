pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps { 
                sh 'echo "Building."'
                sh 'printenv'
            }
        }
        stage('Test'){
            steps { 
                sh 'testing'
            }
        }
        stage('Deploy') {
            steps {
                sh 'deploying'
            }
        }
    }
}
