pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Code checkout stage'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project'
                sh 'docker build -t my-web-project .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the project'
                sh 'docker image inspect my-web-project'
            }
        }
    }
}
