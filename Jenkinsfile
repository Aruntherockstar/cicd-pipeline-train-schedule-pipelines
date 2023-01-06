pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building the automation build"
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
