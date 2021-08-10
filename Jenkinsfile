pipeline {
    agent any
    
    stages {
        stage('clonethecode') {
            steps {
                git 'https://github.com/DilipFidelity/TestDevOps'
            }
        }
        stage('build') {
            steps {
            echo 'build is started'
                sh 
                'javac test.java'
            }
        }
        stage('execute test') {
            steps {
                sh 'echo three'
            }
        }
        stage('approval') {
            steps {
                input 'Approved to Deploy ?'
            }
        }
        stage('deploy') {
            steps {
                sh 'echo deploy'
            }
        }
        
    }
}
