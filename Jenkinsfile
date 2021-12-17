pipeline {
	agent any
		stages {
			stage('First') {
				steps {
					script {
						env.execute = true
					}
					echo "${env.execute}"
					sh '''
						echo "Updating Second Stage"
					'''
				}
			}


			stage('Second')
			when {
				expression {
					env.execute == true
				}
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
