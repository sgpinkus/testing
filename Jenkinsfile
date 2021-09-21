pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps { 
                sh 'echo Building. BRANCH_NAME=${env.BRANCH_NAME}'
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
