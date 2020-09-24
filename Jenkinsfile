pipeline{
    stages{
        stage("build"){
            steps{
                sh ./gradlew build
                archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true
            }   
        }
    }
}
