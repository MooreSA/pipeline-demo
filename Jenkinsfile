Jenkinsfile (Declarative Pipeline)
pipeline {
    agent { docker { image 'node:14-alpine' } }
    stages {
        stage('build') {
            steps 
            retry(3) {
                sh 'npm --version'
            }

            timeout(time: 3, unit: 'MINUTES') {
                sh 'echo "help me"'
            }
        }
    }
}