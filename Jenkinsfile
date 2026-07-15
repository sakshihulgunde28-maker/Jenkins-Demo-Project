
pipeline {

    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out code from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }

        stage('Deploy') {
    steps {
        sh 'cp index.html /var/www/html/'
        echo 'Website deployed successfully'
    }
}
            }
        }

    }

}