pipeline {
    agent {
        kubernetes {
            label 'scala-build-agent'
        }
    }
    
    stages {
            stage('Compile') {
                steps {
                    container('sbt'){
                        echo "Compiling..."
                        sh "sbt compile"
                    }
                }
            }
        stage('Test') {
            steps {
                container('sbt'){
                    echo "Testing..."
                    sh "sbt test"
                }
            }
        }
                stage('Package') {
                    steps {
                        container('sbt'){
                            echo "Packaging..."
                            sh "sbt package"
                        }
                    }
                }
    }
}
