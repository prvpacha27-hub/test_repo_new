pipeline {
    agent any
    stages {
        stage('Checkout java code') {
          steps {
            deleteDir()
            sh "./file2.sh"
            }
        }

        stage('Build') {
            steps {
                sh 'echo Build step here'
            }
        }
    }
}
