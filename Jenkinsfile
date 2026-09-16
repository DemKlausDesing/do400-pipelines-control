node('nodejs') {
    stage('Checkout') {
        // URL anpassen!!!
        git branch: 'main',
            url: 'https://github.com/DemKlausDesing/do400-pipelines-control'
    }

    // Mega-hammer-hart
    stage('Mega') {
        sh 'echo Mega ...'
    }
    
    stage('Backend Tests') {
        sh 'node ./backend/test.js'
    }
    
    stage('Frontend Tests') {
        sh 'node ./frontend/test.js'
    }
}
