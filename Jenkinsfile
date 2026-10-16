pipeline {
    agent any
    stages {
        stage('Checkout java code') {
          steps {
            deleteDir()
            mkdir pra
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
