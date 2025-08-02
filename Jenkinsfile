pipeline {
    agent any

    stages {
        stage('echo stage') {
            steps {
                sh "echo 'Hello world'"
            }
        }
        stage('cat readme') {
            when {
                branch "fix-*"
            }
            steps {
                sh '''
                    cat README.md
                '''
            }
        }
    }
}
