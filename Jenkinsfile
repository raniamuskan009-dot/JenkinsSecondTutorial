pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Project'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing Project'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Project'
            }
        }
    }
    post {
    // Runs regardless of build result
    always {
        echo 'Post build condition running'
    }
    // Runs only if build failed
    failure {
        echo 'Post Action if Build Failed'
    }
}
}






