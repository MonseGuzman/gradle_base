pipeline {
    agent {label 'swarm'}
    stages {
        stage('Build') {
            steps {
                sh 'chmod +x gradle ; ./gradlew clean test --no-daemon'
                sh './gradlew build'
            }
        }
    }
}