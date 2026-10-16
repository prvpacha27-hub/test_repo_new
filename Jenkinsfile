pipeline {
    agent any
    stages {
        stage('Checkout java code') {
          steps {
            deleteDir()
            sh "ls"
            }
        }

        stage('Build') {
            steps {
                sh 'testing'
            }
        }
    }
}
