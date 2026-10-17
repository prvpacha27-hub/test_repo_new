pipeline {
    agent any

    stages {
        stage('Checkout Repository') {
            steps {
                // Clones the exact Git repository and branch where this Jenkinsfile lives
                cleanWs()
		checkout scm
            }
        }
        
        stage('Create Directory') {
            steps {
                // Creates a new directory named 'new_folder' inside the cloned repository workspace
                sh 'mkdir -p java_code_repo'
                
                // Optional: Run a list command to verify the directory was created
                sh 'ls -la'
                sh "chmod +x file2.sh"

                sh "./file2.sh"

            }
        }
        stage('clone repo') {
            steps {
                dir('java_code_repo')
                git branch: 'master',
                //    credentialsId: 'github-creds',
                url: 'https://github.com/Prashanthv10/javaparser-maven-sample.git'                
            }
        }
    }
}
