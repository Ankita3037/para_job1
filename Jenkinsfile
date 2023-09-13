// Jenkins file (Declarative Pipeline)

pipeline {
    agent any
    parameters {
        booleanParam(name: 'ENABLE_FEATURE_X', defaultValue: true, description: 'Enable Feature X')
        booleanParam(name: 'ENABLE_FEATURE_Y', defaultValue: false, description: 'Enable Feature Y')
    }
    stages {
        stage('Build') {
            steps {
                script {
                    if (params.ENABLE_FEATURE_X) {
                        // Execute code for Feature X
                        sh "git --version"
                    }
                    if (params.ENABLE_FEATURE_Y) {
                        // Execute code for Feature Y
                        sh "java --version"
                    }
                }
            }
        }
    }
}
