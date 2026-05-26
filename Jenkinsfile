pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Yahan apni repo ka link daalo
                git branch: 'main', url: 'https://github.com/PraveenKumar1-hub/MY-FIRST-CI-CD-PIPELINE.git'
            }
        }
        stage('Docker Build') {
            steps {
                script {
                    echo 'Building image...'
                    // Ye command check karegi ki Docker image ban rahi hai ya nahi
                    sh 'docker build -t my-test-app .'
                }
            }
        }
    }
}
