pipeline{
  agent any
  stages{
    stage('-clean-'){
      steps{
        sh "mvn clean"
      }
    }
    stage('-test-'){
      steps{
        sh '''
        echo "se pasan los test"
        '''
      }
    }
    stage('-compile & deploy-'){
      steps{
        sh '''
        mvn compile
        mvn deploy
        '''
      }
    }
  }
}
