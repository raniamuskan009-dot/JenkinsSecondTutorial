pipeline {
    agent any

    tools {
        maven 'Maven3'   // must match name in Manage Jenkins → Tools
    }

    environment {
        NEW_VERSION = '1.3.0'
    }

    stages {
        stage('Build') {
            steps {
            
                // Windows — use bat instead of sh:
                bat 'mvn -v'
            }
        }
        // ...other stages
    }
}
