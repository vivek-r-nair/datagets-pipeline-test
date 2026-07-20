pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        sh 'echo Pulling Datagets code from GitHub'
	// The factory is actually open this time
	
      }
    }
    stage('Build'){
      steps{
        sh 'The webhook automatically triggered this build!'
	// Testing the webhook automation
      }
    }
    stage('Test'){
      steps{
        sh 'echo running the tests for datagets code'
	// The door is finally unlocked

      }
    }
  }
  post{
    always{
      sh 'echo pipeline finsished successfully sending email notification'
      // The timeline is fixed!
    }
  }
}
