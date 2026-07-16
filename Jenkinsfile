
node {

    stage('Compile C Program') {

        echo "Compiling C program..."

        sh 'gcc hello.c -o hello'

    }


    stage('Run C Program') {

        echo "Running C program..."

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