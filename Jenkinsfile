pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('Deploy to staging') {
            steps{
            build job: 'deploy-to-staging'
            }
        }
        stage('Deploy to production'){
            steps{
                build job: 'deploy-to-prod'
            }
        }
    }
}
