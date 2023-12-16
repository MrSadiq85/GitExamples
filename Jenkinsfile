pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Run Smoke and Regression test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post {
            always{
                emailext body: 'SUCESS.', subject: 'Pipeline status', to: 'lookingfor7lpa@gmail.com'
            }
        }
}
