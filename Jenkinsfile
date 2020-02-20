pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh 'chmod +x gradlew'
                sh './gradlew clean test --no-daemon'
                sh './gradlew build'
            }
        }
    }
}