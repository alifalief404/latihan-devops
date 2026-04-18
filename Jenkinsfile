pipeline {
    agent any

    stages {
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
