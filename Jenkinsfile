pipeline {
    agent {
        kubernetes {
            label 'scala-build-agent'
        }
    }
    
    stages {
        stage('Build') {
            steps {
                container('sbt'){
                    echo "Cleaning..."
                    sh "sbt clean"
                }
            }
        }
    }
}
