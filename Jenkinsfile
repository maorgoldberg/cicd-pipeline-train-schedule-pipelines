pipeline{
    stages{
        stage("build"){
            steps{
                sh ./gradlew build
                
            }   
        }
    }
    post{
        always{
            archiveArtifacts artifacts: 'dist/trainSchedule.zip', fingerprint: true
        }
    }
}
