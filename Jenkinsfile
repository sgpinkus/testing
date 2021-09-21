pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps { 
                sh 'echo "Building.."'
                sh 'printenv'
                sh 'echo ---------'
                sh 'echo $BRANCH_NAME'
            }
        }
        stage('Test'){
            steps { 
                sh 'echo testing ${GIT_BRANCH}'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo deploying'
            }
        }
    }
}
