pipeline {
    agent any
    stages {
        stage('Clone Repository') {
    steps {
        git branch: 'main', url: 'https://github.com/AkashshivuJk/Jenkins-Automation.git'
    }
}

        stage('Build') {
            steps {
                sh 'chmod +x build.sh'
                sh './build.sh'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
