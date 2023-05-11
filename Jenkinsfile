/* SCRIPTED
node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
}  */
//DECLARATIVE

pipeline{
	agent any
	stages{
		stage('Build'){
			steps{
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Test"
			}
		}
		stage('Integration Test'){
			steps{
				echo "Integration Test"
			}
		}
	}post{
		always{ //POST is used to execute a code once the pipeline is completed
				echo "soy increible" 
		}
		success{ //SUCCESS is used to execute a code once the pipeline is completed sucessesfuly 
				echo "I run when you are successful" 
		}
		fail{ //FAIL is used to execute a code once the pipeline is completed FAIL 
				echo "I run when you failed" 
		}
	}

}
