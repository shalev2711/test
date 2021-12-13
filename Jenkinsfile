pipeline {
    agent any
    stages {
        stage('build') {
            parallel {
                stage('Build A') {
                    steps {
                        echo 'Building A...'
                    }
                } //stage Build A
                stage('build B') {
                    steps {
                        echo 'Building B...'
                    }
                }//stage Build B
            } //parallel
        } //stage build
        stage('Test') {
            steps {
                sh "pip install pytest"
                sh "python3 -m pytest"
            }
        } //stage test
        stage ('Deploy') {
            steps {
                echo 'Deploying....'
            }
        } //stage deploy
    }//stages
    
}//pipeline
