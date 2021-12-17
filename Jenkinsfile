
pipeline {
	agent any
	environment {
		executor_number= "step uno"
		stages {
			stage('First') {
				steps {
					sh '''
						echo "${env.executor_number}"
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
