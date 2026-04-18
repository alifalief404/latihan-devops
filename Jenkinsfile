pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/alifalief404/latihan-devops.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build aplikasi...'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t latihan-devops .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run latihan-devops'
            }
        }
    }
}
