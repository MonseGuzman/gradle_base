pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh 'chmod +x gradle'
                sh './gradlew clean test --no-daemon'
                sh './gradlew build'
            }
        }
    }
}