pipeline{
  agent any
  stages{
    stage('One'){
      steps{
        echo "Hi, this is stage 1."
      }
    }
    stage('Two'){
      steps{
        input('Do you want to proceed?')
      }
    }
    stage('Three'){
      steps{
        when {
          not{
            branch "master"
          }
        }
        steps{
          echo "hello"
        }
      }
    }
  }
}
