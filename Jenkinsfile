pipeline {
    agent {label: "Linux"}
    options {
        buildDiscarder  logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5',
        daystoKeepStr: '', numToKeepStr: '5')
        disabledConcurrentBuild()
    }
    stages {
        stage('Hello') {
            steps {
                echo 'Hello'
            }
        }
    }
}