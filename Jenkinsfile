pipeline {

    agent any

    stages {
        stage("build") {
            steps {
                echo "Building the aplication..."
                sh "./gradlew build --no-daemon"
                archiveArtifacts artifacts: dist/trainSchedule.zip
            }
        }
    } 
}
