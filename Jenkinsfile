pipeline {
    agent { docker { image 'maven:3.6.0' } }
    stages {
        stage('Build') {
            steps {
            bat 'echo "Hello World"'
                bat '''
                    echo "Multiline shell steps works too"
                    dir
                '''
            }
        }
    }
}
