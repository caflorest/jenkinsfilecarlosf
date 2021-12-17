pipeline {
	agent any
	environment {
        DISABLE_AUTH = 'true'
    }
		stages {
			stage('First') {
				steps {
					echo "DISABLE_AUTH is ${DISABLE_AUTH}"
					sh '''
						echo "Updating Second Stage"
					'''
				}
			}


			stage('Second') {
				steps {
					sh '''
						echo "Step Two"
					'''
				}
			} 

			stage('Third') {
				steps {
					sh '''
						echo "Step Three"
					'''
				}
			}
		}
}
