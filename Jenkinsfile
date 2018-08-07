pipeline {
    agent {
        docker {
            image 'node:6'
            args '-p 3000:3000 -v .nmp:/.nmp'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'set -x ; npm install'
            }
        }
    }
}
