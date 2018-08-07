pipeline {
    agent {
        docker {
            image 'node:6'
            args '-p 3000:3000 -v /var/lib/jenkins/workspace/simple-node-js-react-npm-app/.nmp:/.nmp'
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
