pipeline {
    agent any

    tools {
        maven 'Maven'   // must match name in Manage Jenkins → Tools
    }

    environment {
        NEW_VERSION = '1.3.0'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building version ${NEW_VERSION}"
                // Linux / macOS:
                sh "mvn --version"
                // Windows — use bat instead of sh:
                // bat 'mvn --version'
            }
        }
        // ...other stages
    }
}
