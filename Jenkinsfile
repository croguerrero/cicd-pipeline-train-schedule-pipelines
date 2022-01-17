pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build '
                sh './gradlew zip '
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}