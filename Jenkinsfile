pipeline {
    agent any
    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/Manohar-mattepu/ecomm.git'
            }
        }
        stage('Copy HTML') {
            steps {
                sh '''
                    mkdir -p html_output
                    cp index.html html_output/
                '''
            }
        }
    }
}
