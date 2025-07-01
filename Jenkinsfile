pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Manohar-mattepu/ecomm.git'
            }
        }
        stage('Copy HTML') {
            steps {
                // avoid sudo and use a directory Jenkins owns
                sh 'mkdir -p /home/jenkins/html && cp index.html /home/jenkins/html/'
            }
        }
    }
}
