// pipeline {
//     agent any
//     stages {
//         stage('Build') {
//             steps {
//                 sh 'echo Im bulidling my pipeline throug scm'
//             }
//         }
//         stage('Test'){
//             steps {
//                 sh 'echo testing my pipeline throug scm'
                
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 sh 'echo  im deploying my pipeline throug scm' 
//             }
//         }
//     }
// }    

pipeline {
    agent {
        label 'AGENT-1'
    }
        parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
 
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
 
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
 
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
 
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {
        stage('Build') {
            steps {
                sh ''
            }
        }
        stage('Test') {
            steps {
                sh 'echo this is test'
            }
        }
        stage('Deploy') {
            steps {
                sh """
                sh 03-variable.sh
                """
            }
        }
    }
}