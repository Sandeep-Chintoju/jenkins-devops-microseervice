pipeline{
	agent any
	// agent { docker { image 'maven:3.6.3'} } 
		stages {
			stage('Build') {
				steps {
					echo "Build"
					echo "PATH is $env.PATH"
					echo "BUILD_NUMBER is $env.BUILD_NUMBER"
					echo "BUILD_ID is $env.BUILD_ID"
					echo "JOB_NAME is $env.JOB_NAME"
					echo "BUILD_TAG is $env.BUILD_TAG"
					echo "BUILD_URL is $env.BUILD_URL"

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
				echo 'i am awesome. I run always'
			}
			success {
				echo 'i run when you are successful'
			}
			failure {
				echo 'i run whaen you fail'
			}
			changed {
				echo 'i run when you change'
			}
		}
}
