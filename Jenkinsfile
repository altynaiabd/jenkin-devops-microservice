pipeline {
	// agent any
	agent { docker { image 'node:21.6' } }
	stages {
		stage('Build') {
			steps {
				sh "node --version"
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
			echo "Im awesome. I always run"
		}
		success {
			echo "I run when you are successfull"
		}
		failure {
			echo "I run when you fail"
		}
	}
}
