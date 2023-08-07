node {
    // Menggunakan docker agent dengan image node:16-buster-slim dan port 3000:3000
    docker.image('node:16-buster-slim').withRun('-p 3000:3000 --privileged') {
        stage('Preparation') {
            // Instal npm di dalam kontainer
            sh 'apt-get update && apt-get install -y npm'
        }
        stage('Build') {
            // Langkah-langkah untuk tahap build
            sh 'npm install'
        }
    }
}