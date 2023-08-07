pipeline{
  agent any
  stages{
    stage("Maven build"){
      steps{
        echo "Thisis Jenkinsfile"
      }
    }
    stage("Dev deploy"){
      steps{
        when{
          branch "develop"
        }
        echo "Deploy to develop"
      }
    }
    stage("test deploy"){
      steps{
        when{
          branch "test"
        }
        echo "deploy to test"
      }
    }
    stage("prod deploy"){
      steps{
        when{
          branch "main"
        }
        echo "ddeploy to main"
      }
    }
  }
}
