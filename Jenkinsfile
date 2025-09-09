pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/playwright:v1.55.0-noble'
        }
    }

    stages {
        stage('Node.js Deps') {
            steps {
                sh 'npm install'
            }
        }
        stage('E2E Testss') {
            steps {
                sh 'npx playwright test'
            }
        }
    }
}
