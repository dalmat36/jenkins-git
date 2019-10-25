pipeline {
    agent any
    environment {
    SBT_HOME =  tool name: 'sbt-1.2.8', type: 'org.jvnet.hudson.plugins.SbtPluginBuilder$SbtInstallation'
    }
    stages {
        stage('Build') {
            steps {
                echo "Cleaning..."
                sh "${SBT_HOME}/bin/sbt clean"
            }
        }
    }
}
