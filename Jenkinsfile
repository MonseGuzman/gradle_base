pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh './gradlew clean test --no-daemon'
                sh './gradlew build'
            }
        }
    }
}