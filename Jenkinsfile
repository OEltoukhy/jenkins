pipeline{
  agent any
  environment{
    NEW_VERSION = "1.3.0"
  }

  stages{
    stage("test"){
      steps{
      echo "testing...."
      echo "the new version is: ${NEW_VERSION}"
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
