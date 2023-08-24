pipeline{
	agent any
	environment {
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH="$dockerHome/bin:$mavenHome/bin:$PATH"
	}
 stages{
	 stage('build'){
         steps{
			sh 'maven --version'
			sh 'docker version'
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
