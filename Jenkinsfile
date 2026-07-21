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
    stage('Approve Production Deployment') {
            steps {
                script {
                    timeout(time: 5, unit: 'MINUTES') {
                        input(
                            message: "Deploy Demo to PRODUCTION?",
                            ok: "Approve Deployment"
                        )
                    }
                }
            }
        }
    stage('Deploy'){
      steps{
        sh  "echo Deploying Datagets Build v${BUILD_NUMBER} to the Production Server!"

      }
    }
  }
  post{
   
        success {
            sh "echo  SUCCESS: Build v${BUILD_NUMBER} deployed safely. Notifying the Product Team!"
        }
        failure {
            sh "echo  FAILED: The pipeline broke. Sending emergency alert to the Engineering Team!"
        }
    }
 
}
