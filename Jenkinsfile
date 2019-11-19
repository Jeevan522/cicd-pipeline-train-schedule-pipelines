pipeline{
  agent any{
      stages{
        stage{'Build'}{
          steps{
            echo 'running the Jenkins automation task'
            sh './gradlew build --no-deamon'
            archiveArtifacts artifacts: 'dist/trainSchedule.zip'
           }
        }
      }
   }
