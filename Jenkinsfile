pipeline {
	agent any 
	
	environment {
		dockerHome = tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	
	stages {

	stage('Build') {
		steps {
			sh 'mvn --version'
		echo "Build"
			
		}
	}
		
	stage('Test') {
		steps {
			
		echo "Test"
			
		}
	}
		
	stage('Integration Test') {
		steps {
			
		echo "Integration Test"
			
		}
	}
}
	
	post {
		always {
			echo 'I execute alwats'
		}
		success {
			echo 'I run when you are successfull'
		}
		failure {
			echo 'I run when you are failed'
		}
		
	}
	
}
