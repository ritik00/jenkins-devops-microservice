pipeline{
	agent any
 stages{
	 stage('build'){
         steps{
			echo "build"
		 }		
	 }
	 stage('test'){
         steps{
			echo "test"
		 }		
	 }
	 stage('integration test'){
         steps{
			echo "integration test"
		 }		
	 }
 }
 post{
	always{
		echo "always"
	}
	success {
		echo "success"
	}
	failure {
		echo "failure"
	}
 }
}
