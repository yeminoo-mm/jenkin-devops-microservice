// SCRIPTED

// DECLARATIVE
pipeline {
	agent any
	// agent { docker { image 'maven:3.6.3'}}
	// agent { docker { image 'node:13.8'}}
	stages {
		stage('Build') {
			steps {
				// sh "mvn --version"
				// sh "node --version"
				echo "Build"
				echo "$PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "$env.BUILD_ID"
				echo "$env.JOB_NAME"
				echo "$env.BUILD_TAG"
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
	
//	post {
		always {
			echo 'I am awesome. I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
// }