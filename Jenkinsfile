pipeline {
    agent { docker { image 'python:3.10.1-alpine' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
      stage('Test') {
        sh "pip install pytest"
        sh "python3 -m pytest"
        
      }
    }
}
