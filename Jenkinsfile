pipeline {
    agent any
    tool name: 'sbt-1.2.8', type: 'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation'
    stages {
        stage('Build') {
            steps {
                echo "Cleaning..."
                sh "/usr/local/bin/sbt clean"
            }
        }
    }
}
