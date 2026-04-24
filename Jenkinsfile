flag=true

pipeline {
    agent any
    stages {
        stage('Build') {
            steps { echo 'Building Project' }
        }
        stage('Test') {
            when {
                expression {
                    flag == false   // change to true to run test
                }
            }
            steps { echo 'Testing Project' }
        }
        stage('Deploy') {
            steps { echo 'Deploying Project' }
        }
    }
}
