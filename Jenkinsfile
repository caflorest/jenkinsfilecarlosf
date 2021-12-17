pipeline {
	agent any
	environment {
        DISABLE_AUTH = 'true'
    }
		stages {
			stage('One') {
				steps {
					echo "DISABLE_AUTH is ${DISABLE_AUTH}"
					sh '''
						echo "Step One"
					'''
				}
			}


			stage('Two') {
				steps {
					sh '''
						echo "Step Two"
					'''
				}
			} 

			stage('Three') {
				steps {
					sh '''
						echo "Step Three"
					'''
				}
			}
		}
}
