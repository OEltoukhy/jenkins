pipeline{
  agent any

  stages{
    stage("test"){
      steps{
      echo "testing...."
      }
    }

    stage("build"){
      // when{
      //   expression{
      //     BRANCH_NAME == "origin/main"
      //   }
      // }
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
    success{
            echo "the build is done sucessfully"
  }
    failure{
      echo "There is an error please try to fix it"
    }
  }
}
