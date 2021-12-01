pipeline {
	agent any
	stages {
		stage('Checkout SCM') {
			steps {
				echo "Checkout SCM"
			}
		}

		stage('OWASP DependencyCheck') {
			steps {
				dependencyCheck additionalArguments: '--format HTML --format XML', odcInstallation: 'Default'
			}
		}
	}	
	post {
		success {
			echo "hihi"
		}
	}
}
