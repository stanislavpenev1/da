pipeline{
agent any
  stages{
    stage("Build"){
      steps{
      echo "Hello from build"
    }
    } stage("test"){
      steps{
      echo "Hello from test"
      }
    }
  }post{
    always{
          echo "shutdown machine"
    }
    success{
          echo"send emails for success"
    }
    failure{
          echo"send emails for failure"
    }
  }
}
