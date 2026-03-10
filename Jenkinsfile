pipeline {
    agent any

    tools {
        nodejs "node18"
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/dineshvit11/reactmonoapp.git'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }

    }
}
