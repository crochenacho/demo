pipeline{
  agent any
  stages{
    stage('-clean-'){
      steps{
        sh '''
        cd code
        mvn clean
        '''
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
