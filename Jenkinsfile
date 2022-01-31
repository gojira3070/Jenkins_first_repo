pipeline {
    agent any
    stages {
        stage('clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/gojira3070/Jenkins_first_repo.git"
            }
        }
        stage('build') {
            steps {
                sh "cd Jenkins_first_repo/ && javac Main.java"
            }
        }
        stage('run') {
            steps {
                sh "cd Jenkins_first_repo/ && java Main"
            }
        }
    }
} 
