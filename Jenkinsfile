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
        sh 'echo The webhook automatically triggered this build!'
	// Testing the webhook automation
      }
    }
    stage('Test'){
      steps{
        sh 'echo running the tests for datagets code'
	// The door is finally unlocked

      }
    }
    stage('Deploy'){
      steps{
        sh  "echo Deploying Datagets Build v${BUILD_NUMBER} to the Production Server!"

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
