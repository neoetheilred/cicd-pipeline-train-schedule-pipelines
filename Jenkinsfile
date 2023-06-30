pipeline {
    agent any
    stages {
        stage('build gradlew') {
            steps {
                echo "Building..."
                sh "./gradlew build --no-daemon"
                archiveArtifacts artifacts: "dist/trainSchedule.zip"
            }
        }
    }
}