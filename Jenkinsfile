node {
    docker.image('node:16-buster-slim').inside {
        stage('Preparation') {
            sh 'apt-get update && apt-get install -y nodejs npm'
        }
        stage('Build'){
            sh 'npm install'
        }
        stage('Test'){
            sh './jenkins/scripts/test.sh'
        }
    }
}