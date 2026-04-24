pipeline {
    agent any

    environment {
        // Accessible by all stages
        NEW_VERSION = '1.3.0'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building Project'
                // Use " " (double quotes) to interpolate variables
                echo "Building version ${NEW_VERSION}"
            }
        }
        // ...other stages
    }
}
