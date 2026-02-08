pipeline {
    agent { label 'docker-agent' }

    options {
        buildDiscarder(logRotator(numToKeepStr: '5'))
        timestamps()
    }

    stages {
        stage('Verify Agent') {
            steps {
                echo 'Build running on remote Docker agent'
                sh 'java -version'
            }
        }

        stage('System Info') {
            steps {
                sh 'uname -a'
                sh 'whoami'
            }
        }

        stage('Build Simulation') {
            steps {
                sh 'echo "Simulating project build..."'
                sh 'sleep 5'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
