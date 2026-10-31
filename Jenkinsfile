pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                echo 'Repository cloned successfully!'
            }
        }

        stage('Verify') {
            steps {
                bat 'echo Verifying project...'
                bat '"E:\\DevStorage\\src\\git\\cmd\\git.exe" status'
            }
        }

        stage('List Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Simulated Deploy') {
            steps {
                echo 'Deployment completed successfully!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline finished successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}