pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon -x npm_test'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
