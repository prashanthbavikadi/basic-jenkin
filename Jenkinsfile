pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                sh 'Im bulidling my pipeline throug scm '
            }
        }
        stage('Test'){
            steps {
                sh 'Im testing my pipeline throug scm'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'Im deploying my pipeline throug scm' 
            }
        }
    }
}