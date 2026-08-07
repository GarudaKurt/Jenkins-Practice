pipeline {
    agent any
    options {
        buildDiscarder  logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5',
        daysToKeepStr: '', numToKeepStr: '5')
        disableConcurrentBuilds()
    }
    stages {
        stage('Hello') {
            steps {
                echo "hello"
            }
        }
<<<<<<< Updated upstream
=======
        stage('cat README') {
            when {
                branch "fix-*"
            }
            steps {
                sh '''
                    cat README.md
                '''
            }
        }
        stage('Build'){
            when {
                branch "main"
            }
            steps {
                echo "Building on main..."
            }
            sh '''
                # replace with your actual build command, e.g.:
                # mvn clean package
                # npm install && npm run build
                echo "build step placeholder"
            '''
        }
        stage('Test') {
            when {
                branch "main"
            }
            steps{
                echo "Testing main branch.."
            }
            echo '''
                # replace with your actual build command, e.g.:
                # mvn clean package
                # npm install && npm run build
                echo "build step placeholder"
            '''
        }
>>>>>>> Stashed changes
    }
}