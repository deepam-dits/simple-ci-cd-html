pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/deepam-dits/simple-ci-cd-html.git', branch: 'main'
            }
        }
        stage('Build') {
            steps {
                echo 'No build needed for static HTML.'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying index.html to local folder...'
                bat 'mkdir C:\\JenkinsDeploy || exit 0'
                bat 'copy index.html C:\\JenkinsDeploy\\index.html /Y'
            }
        }
    }
}
