pipeline {
	agent any
	environment {
        execute = "true"
    }
		stages {
			stage('First') {
				steps {
					echo "${env.execute}"
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
