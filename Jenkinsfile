node {
    // Menggunakan docker agent dengan image node:16-buster-slim dan port 3000:3000
    docker.image('node:16-buster-slim').withRun('-p 3000:3000') {
        stage('Build') {
            // Langkah-langkah untuk tahap build
            sh 'npm install'
        }
    }
}