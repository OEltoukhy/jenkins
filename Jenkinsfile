pipeline{
  agent any

  stages{
    stage("test"){
      steps{
      echo "testing...."
      }
    }

    stage("build"){
      steps{
      echo "building...."
      }
    }

    stage("deploy"){
      steps{
      echo "deploying...."
      }
    }
  }
  post{
    always{
      echo "the build is done"
    }
    sucess{
            echo "the build is done sucessfully"
  }
    failure{
      echo "There is an error please try to fix it"
    }
}
