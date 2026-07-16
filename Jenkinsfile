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