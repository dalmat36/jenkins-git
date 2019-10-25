pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Cleaning..."
                sh "/usr/local/bin/sbt clean"
            }
        }
    }
}
