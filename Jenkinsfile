pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                bat '''
                echo ===== Jenkins Workspace =====
                cd
                dir
                '''
            }
        }

        stage('Test') {
            steps {
                bat '''
                echo ===== Printing file =====
                type hello.txt
                '''
            }
        }

        stage('Done') {
            steps {
                echo '✅ Pipeline executed successfully'
            }
        }
    }
}
