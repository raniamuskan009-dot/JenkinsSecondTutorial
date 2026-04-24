pipeline {
    agent any

    tools {
        maven 'Maven3'   // must match name in Manage Jenkins → Tools
    }


    stages {
        stage('Build') {
            steps {
                echo "Building version ${NEW_VERSION}"
                // Linux / macOS:
                bat "mvn -v"
                // Windows — use bat instead of sh:
                // bat 'mvn --version'
            }
        }
        // ...other stages
    }
}

parameters {
    // Free-text input
    string(
        name: 'VERSION',
        defaultValue: '',
        description: 'version to deploy on prod'
    )
    // Dropdown / choice
    choice(
        name: 'VERSION',
        choices: ['1.1.0', '1.2.0', '1.3.0'],
        description: ''
    )
    // Boolean toggle
    booleanParam(
        name: 'executeTests',
        defaultValue: true,
        description: ''
    )
}
