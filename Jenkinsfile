pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/dev25074382/securepay-cicd.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Build Successful'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}