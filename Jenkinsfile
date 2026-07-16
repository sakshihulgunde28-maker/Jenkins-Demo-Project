
node {

    stage('Checkout') {
        checkout scm
    }

    stage('Check Files') {
        sh 'pwd'
        sh 'ls -la'
    }

    stage('Compile C Program') {
        sh 'gcc hello.c -o hello'
    }

    stage('Run C Program') {
        sh './hello'
    }
}



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