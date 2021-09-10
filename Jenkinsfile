pipeline{
	agent any 
		stages {
			stage('Build') {
				steps {
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
