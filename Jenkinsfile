
pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						 env.variable="step one"
				
					sh '''
						echo "${env.variable}"
					'''
					}
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
