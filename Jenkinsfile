pipeline{
  agent any
  stages{
    stage("Maven build"){
      steps{
        echo "Thisis Jenkinsfile"
      }
    }
    stage("Dev deploy"){
       when{
          branch "develop"
        }
      steps{
        echo "Deploy to develop"
      }
    }
    stage("test deploy"){
       when{
          branch "test"
        }
      steps{
        echo "deploy to test"
      }
    }
    stage("prod deploy"){
      when{
          branch "main"
        }
      steps{
        echo "ddeploy to main"
      }
    }
  }
}
